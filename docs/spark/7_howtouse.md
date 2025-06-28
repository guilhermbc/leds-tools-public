---
sidebar_position: 7
title: How to Use
---

## Option 1: Via VSCode Extension

Ensure that the **Leds - Spark - Beta** extension is installed in your VSCode. This extension is available through the editor's built-in extension marketplace. It is required to leverage Spark's features without the need to import libraries locally into your project.

Note that it differs from the **Spark - LEDS** extension, which is also available in the same marketplace. Unlike the latter, **Leds - Spark - Beta** relies on an external library that unifies backend and frontend generation, with a greater decoupling of responsibilities from Langium. The library, in turn, decouples business logic from the extension’s core repository, enabling reuse without compromising the main generation functionality.

### Steps:

1. Create a file with the `.spark` extension  
   Example: `slave_one.spark`
   
2. Define the [class diagram](6_lang.md)  

3. Save the `.spark` file

4. Right-click the file** and choose one of the available generation options from the context menu.  
   ![Menu com opções de geração ao clicar com botão direito](./img/right-click.png)

5. Spark will generate the software artifacts.  
   ![Exemplo de hierarquia de pastas gerada](./img/folders.png)

---

## Option 2: Via Command-Line Interface (CLI)

Alternatively, you can install the Spark package using a Node package manager. You must have one of these managers installed on your operating system. It is recommended to use **npm** version 5.2.0 or higher.

Once npm is installed, follow these steps to complete the generation:

### Steps:

1. Install the Spark npm package via the terminal:

    ```bash
    npm i spark-leds-beta@latest
    ```

2. Create a .spark file as previously described, in the directory where you wish to generate the files.

3. Execute the generation command via the terminal:
    ```bash
    npx spark-cli generate ./path/to/a/spark/file
    ```

