Tic Tac Toe
===========

A simple command-line Tic-Tac-Toe game implemented in Java.

**Java Version**: Java 21 (LTS)

**Contents**
- `src/main/java` — Java source files
- `pom.xml` — Maven build file (project configured for Java 21)

**Quick Start (Windows PowerShell)**

Prerequisites:
- JDK 21 installed (the project was verified with `C:\Users\Admin\.jdk\jdk-21.0.8`).
- Optional: Maven if you prefer `mvn` runs.

1) Set `JAVA_HOME` and add `javac`/`java` to your PATH (persist for future shells):

```powershell
[Environment]::SetEnvironmentVariable('JAVA_HOME','C:\Users\Admin\.jdk\jdk-21.0.8','User')
$userPath = [Environment]::GetEnvironmentVariable('Path','User')
if ($userPath -notlike "*C:\\Users\\Admin\\.jdk\\jdk-21.0.8\\bin*") {
  [Environment]::SetEnvironmentVariable('Path',$userPath + ';C:\Users\Admin\.jdk\jdk-21.0.8\bin','User')
}
```

2) Compile & run directly with `javac`/`java`:

```powershell
cd "C:\Users\Admin\OneDrive\Desktop\tic-tac-toe\src\main\java"
javac Main.java
java Main
```

3) Or build with Maven (if installed):

```powershell
cd "C:\Users\Admin\OneDrive\Desktop\tic-tac-toe"
# compile
mvn clean compile
# run using exec plugin
mvn -q exec:java -Dexec.mainClass="Main"
```

**Notes**
- The repository was upgraded to Java 21 using OpenRewrite and the `pom.xml` was updated accordingly.
- If you encounter `javac`/`java` not found errors, ensure `JAVA_HOME` and the JDK `bin` are in your PATH or use the full path to the executables.

**Contributions**
- Create a new branch, make changes, and open a pull request against `main`.

**License**
- (No license specified)
