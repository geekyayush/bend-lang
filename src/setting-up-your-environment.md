# Chapter 1: Setting Up Your Environment

Welcome to the first chapter of the Unofficial Bend Programming Language Guide. This chapter will guide you through setting up your development environment to start coding in Bend. By the end of this chapter, you'll have the tools you need to write, compile, and run Bend programs on your machine.

## Installing Bend

Before we can start writing Bend code, we need to install the Bend compiler and its runtime environment. Bend is built on top of Rust, so you'll need to have Rust installed on your system. Here's how you can get everything set up:

### Step 1: Install Rust

Bend requires the Rust programming language. To install Rust, follow these steps:

1. Visit the Rust website at https://www.rust-lang.org/tools/install.
2. Follow the instructions to download and install Rust using `rustup`, which is Rust's installation and version management tool.

### Step 2: Install Bend

With Rust set up, you can now install Bend. Open a terminal and run the following commands:

```sh
cargo install hvm
cargo install bend-lang
```

This will install both the HVM2 runtime and Bend language compiler.

### Step 3: Verify Installation

To ensure that Bend has been installed correctly, run:

```sh
bend --help
```

You should see a list of available commands and options for the Bend compiler.

## Editor and IDE Recommendations

While you can write Bend code in any text editor, using an editor with Rust support will make your life easier due to syntax highlighting and other helpful features. Here are some recommendations:

- Visual Studio Code with the Rust extension
- IntelliJ IDEA with the Rust plugin
- Sublime Text with Rust Enhanced package

## Setting Up Your First Project

Create a new directory for your Bend project and navigate into it:

```sh
mkdir bend_project
cd bend_project
```

Inside this directory, create a new file named `main.bend` which will be our entry point for Bend programs.

```sh
touch main.bend
```

Open `main.bend` in your text editor and type in the following code:

```python
# main.bend
def main():
  return "Hello, Bend!"
```

## Compiling and Running Your Code

To compile and run your Bend program, you'll use the `bend` command followed by the `run` subcommand and the file name:

```sh
bend run main.bend
```

You should see the output `Hello, Bend!` in your terminal.

Congratulations! You've successfully set up your Bend development environment, written a simple program, and executed it. In the next chapter, we'll dive into the basics of the Bend programming language and start writing some real code.

---

This concludes Chapter 1 of the guide. Make sure to follow each step carefully to ensure a smooth setup process. Happy coding in Bend!
