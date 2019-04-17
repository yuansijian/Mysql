# Mysql
web端操作自己的mysql   
SQL界面：
使用CodeMirror插件作为在线编辑器。然后将text里面的语句传到post到Processing再赚到function的SqlTable处理。   
先将语句通过split开，再逐条执行。 
let sql = editor.getValue().replace(/\t|\r|\n/g," ").split(";").filter  
若无结果集会提示操作成功或失败，
若有结果集，会返回结果，失败返回错误信息。  
语句一条一条执行，结果集也是一个个生成。最终返回渲染。   
