###  JavaServlet

+ 注意事项`pom.xml`配置该项

  ```xml
  <build>
          <!-- 资源处理 -->
          <resources>
              <resource>
                  <!-- 所在目录 -->
                  <directory>src/main/java</directory>
                  <!-- 包括目录下的 .properties,.xml文件都会扫描到 -->
                  <includes>
                      <include>**/*.properties</include>
                      <include>**/*.xml</include>
                  </includes>
                  <!-- filtering 选项false 不启用过滤器,*.properties 已经起到过滤作用了  -->
                  <filtering>false</filtering>
              </resource>
          </resources>
      </build>
  ```

+ `database.properties`建立在`src/main/resources`文件夹下