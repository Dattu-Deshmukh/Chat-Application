# Chat-Application

A simple Java-based Chat Application for real-time messaging.

## Features

- Real-time text chat between multiple users
- Simple and intuitive user interface

## Getting Started

### Prerequisites

- Java 8 or newer
- [Maven](https://maven.apache.org/) or [Gradle](https://gradle.org/) (if your project uses one)

### Installation(Method1)

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Dattu-Deshmukh/Chat-Application.git
   cd Chat-Application
   ```

## Running(Manual Method)

 1. **Compile Your Code**

Open a terminal in your project root and run:
```sh
javac -d out "chatting Application\src\chatting\application\Client.java" "chatting Application\src\chatting\application\Server.java"
```

 2. **Copy the Icons Folder**

Copy the `icons` folder to your output directory:
```sh
xcopy "chatting Application\src\icons" out\icons /E /I /Y
```

 3. **Run the Server**

Open a terminal and run:
```sh
java -cp out chatting.application.Server
```

 4. **Run the Client**

Open another terminal and run:
```sh
java -cp out chatting.application.Client
```

> **Note:**  
> Always start the server first, then the client.  
> Only use the "Send" button after the client is connected.

---

## Packaging for Distribution

### **Create Executable JAR Files**

**For the Server:**
```sh
jar --create --file Server.jar --main-class chatting.application.Server -C out .
```

**For the Client:**
```sh
jar --create --file Client.jar --main-class chatting.application.Client -C out .
```

- Place the `icons` folder in the same directory as your JAR files, or package them inside the JAR if needed.

---

 How to Run the JARs

- **Start the server:**  
  ```sh
  java -jar Server.jar
  ```
- **Start the client:**  
  ```sh
  java -jar Client.jar
  ```

---

 Notes

- Users must have Java installed to run the JARs.
- For creating a Windows `.exe`, use [Launch4j](http://launch4j.sourceforge.net/).

---
### Troubleshooting

**ClassNotFoundException**
- Make sure all necessary files are compiled.
- If using Maven/Gradle, ensure all dependencies are installed and included in your classpath.
- Double-check the class name and package in the error message.
- Clean and rebuild your project.

If you still have issues, please provide the full error message for detailed help.

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

