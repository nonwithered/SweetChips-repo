# SweetChips-repo

这是SweetChips项目的二进制代码仓库。

Gradle用户可以这样配置：

``` groovy
buildscript {
    repositories {
        maven { url 'https://raw.githubusercontent.com/nonwithered/SweetChips-repo/v0.0.3' }
    }
}
allprojects {
    repositories {
        maven { url 'https://raw.githubusercontent.com/nonwithered/SweetChips-repo/v0.0.3' }
    }
}
```

Maven用户可以这样配置：

``` xml
<repositories>
    <repository>
        <id>SweetChips-repository</id>
        <url>https://raw.githubusercontent.com/nonwithered/SweetChips-repo/v0.0.3</url>
    </repository>
</repositories>
<pluginRepositories>
    <pluginRepository>
        <id>SweetChips-pluginRepository</id>
        <url>https://raw.githubusercontent.com/nonwithered/SweetChips-repo/v0.0.3</url>
    </pluginRepository>
</pluginRepositories>
```

但是这种方式也许会比较缓慢，您也可以选择在您的项目根目录下执行以下命令：

``` bash
git clone -b v0.0.3 git@github.com:nonwithered/SweetChips-repo.git
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
