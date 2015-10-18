Jadler JDK stub server
======================
[Jadler](https://github.com/jadler-mocking/jadler/wiki) by default uses Jetty as an implementation for a stub server
which is problematic especially when you want to use different version of Jetty in you application. Luckily, JDK contains
basic HTTP server which can be used instead. This project will cease to exist once this
[pull request](https://github.com/jadler-mocking/jadler/pull/90) is merged. let's hope it will be soon enough.

# How to use

Include maven dependency

    <dependency>
        <groupId>net.javacrumbs.jadler-jdk</groupId>
        <artifactId>jadler-jdk</artifactId>
        <version>1.1.2</version>
    </dependency>

Enjoy

    import net.javacrumbs.jadler.stubbing.server.jdk.JdkStubHttpServer;

    ...


    initJadlerUsing(new JdkStubHttpServer())