## maven配置

# setting.xml有效性问题    

在默认情况下, 在${MAVEN_HOME}/conf目录下setting.xml为全局设置，运行时在linux用户默认目录下会生成.m2目录，可以将setting.xml拷贝到该目录下，按自己的需要修改设置即可    
# 代理问题  
    <settings>
      ...
      <proxies>
        <proxy>
          <id>my-proxy</id>
          <active>true</active>
          <protocol>http</protocol>
          <host>10.10.1.11</host>
          <port>8081</port>
          <username>****</username>
          <password>****</password>
          <nonProxyHosts>reposity.mycom.com|*.google.com</nonProxyHosts>
        </proxy>
      </proxies>
      ...
    </settings>
