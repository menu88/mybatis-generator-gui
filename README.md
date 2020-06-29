
 自助构建

  ```bash
  git clone https://github.com/menu88/mybatis-generator-gui
  cd mybatis-generator-gui
  mvn jfx:jar
  cd target/jfx/app/
  java -jar mybatis-generator-gui.jar
  ```

 IDE中运行

  Eclipse or IntelliJ IDEA中启动, 找到`com.zzg.mybatis.generator.MainUI`类并运行就可以了（主要你的IED运行的jdk版本是否符合要求）

* 方法四：打包为本地原生应用，双击快捷方式即可启动，方便快捷

  如果不想打包后的安装包logo为Java的灰色的茶杯，需要在pom文件里将对应操作系统平台的图标注释放开

  ```bash
  #<icon>${project.basedir}/package/windows/mybatis-generator-gui.ico</icon>为windows
  #<icon>${project.basedir}/package/macosx/mybatis-generator-gui.icns</icon>为mac
  mvn jfx:native
  ```

