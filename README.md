# gdx-testing

This is a library to enable unit tests in libGDX projects which require testing with JUnit and Mockito.

## Maven
```xml
<dependency>
    <groupId>com.harium.gdx</groupId>
    <artifactId>test</artifactId>
    <version>1.0.0</version>
    <scope>test</scope>
</dependency>
```

## Gradle
```
testImplementation 'com.harium.gdx:test:1.0.0'
```

## Configuration

Whenever you require a headless libGDX environment for your tests to pass, copy the [tests/src/de/tomgrill/gdxtesting/GdxTestRunner.java](tests/src/de/tomgrill/gdxtesting/GdxTestRunner.java) file to your tests project and annotate your test class with:

```java 
@RunWith(GdxTestRunner.class)
public class MySuperTestClass {
	@Test
	public void bestTestInHistory() {
	
	}
}
```

Happy testing!

## License

The gdx-testing project is licensed under the Apache 2 License, meaning you can use it free of charge, without strings attached in commercial and non-commercial projects.

## Source & inspired by

http://shahmirj.com/blog/getting-junit-working-with-libgdx-in-gradle

http://badlogicgames.com/forum/viewtopic.php?f=17&t=1485
