# Mysql
web端操作自己的mysql   
数据库信息部分：   
连接：mysqli_get_host_info($con)   
版本：mysqli_get_server_info($con) 
版本协议：$con->protocol_version   
当前用户：if($result = $conn->query('SELECT USER()')) {   
    echo mysqli_fetch_array($result)['USER()'] ."\n";   
}
Mysql 安装路径：	if($row = $con->query("select @@basedir as basePath from dual;")->fetch_array(MYSQLI_NUM))   
                                echo $row[0];   
Mysql 数据文件路径：if($row = $con->query("show global variables like \"%datadir%\";")->fetch_assoc())   
                                echo $row["Value"];   


SQL界面：
