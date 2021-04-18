# SweetChips-repo

这是SweetChips项目的二进制代码仓库。

Gradle用户可以这样配置：

``` groovy
buildscript {
    repositories {
        maven { url 'https://raw.githubusercontent.com/nonwithered/SweetChips-repo/master' }
    }
}
allprojects {
    repositories {
        maven { url 'https://raw.githubusercontent.com/nonwithered/SweetChips-repo/master' }
    }
}
```

Maven用户可以这样配置：

``` xml
<repositories>
    <repository>
        <id>SweetChips-repository</id>
        <url>https://raw.githubusercontent.com/nonwithered/SweetChips-repo/master</url>
    </repository>
</repositories>
<pluginRepositories>
    <pluginRepository>
        <id>SweetChips-pluginRepository</id>
        <url>https://raw.githubusercontent.com/nonwithered/SweetChips-repo/master</url>
    </pluginRepository>
</pluginRepositories>
```

但是这种方式也许会比较缓慢，您也可以选择在您的项目根目录下执行以下命令：

``` bash
git clone git@github.com:nonwithered/SweetChips-repo.git
```

然后添加以下配置：

Gradle用户可以这样配置：

``` groovy
buildscript {
    repositories {
        maven { url 'SweetChips-repo' }
    }
}
allprojects {
    repositories {
        maven { url 'SweetChips-repo' }
    }
}
```

Maven用户可以这样配置：

``` xml
<repositories>
    <repository>
        <id>SweetChips-repository</id>
        <url>file://SweetChips-repo</url>
    </repository>
</repositories>
<pluginRepositories>
    <pluginRepository>
        <id>SweetChips-pluginRepository</id>
        <url>file://SweetChips-repo</url>
    </pluginRepository>
</pluginRepositories>
```

相关项目：

- [SweetChips](https://github.com/nonwithered/SweetChips)
