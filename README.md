1、代码管理工具：git  

2、版本迭代
每一个版本对应三个分支：feature-v$，feature-v$-dev，feature-v$-rel（其中$为1，2，3，...，表示不同版本的版本号）
feature-v$：表示开发版本
feature-v$-dev：表示FC版本
feature-v$-rel：表示RC版本

研发在开发过程中的需求代码都提交到feature-v$分支上，当项目需要进行FC测试的时候，将feature-v$分支的提交merge到feature-v$-dev分支上，然后出FC包进行测试，当FC测试完成之后，将feature-v$-dev的提交merge到feature-v$-rel分支上进行RC测试。

3、在线自动化打包：Jenkins  
