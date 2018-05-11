title: Hello World
subtitle: Your First Program
theme: league

% TODO update screenshots for Windows UI

# Project Setup

## Let's Launch Eclipse

<div float="right"><img src="./resources/eclipse-426x100.png" class="logo" /></div>
  
Eclipse is our **I**ntegrated **D**evelopment **E**nvironment (**IDE**). IDEs integrate common development tasks with our editor.

Accept the default for workspace. (More on that later.)

## Create a Java Project

% TODO <em> below should probably be a caption class

<div class="sidebar">
	<img alt="New Java Project" src="./resources/new-java-project.png" />
	<p><em>(Yours will look a bit different.)</em></p>
</div>

% fake list, since lists don't 'float' properly

• From the *File* Menu, select *New > Java Project*.

• Specify a *Project name* of *hello-world* as in the screenshot.

• Click the *Finish* button.

## Create a Java Class

<div class="sidebar">
	<img alt="New Java Class" src="./resources/new-java-class.png" />
</div>

• Select the newly created `hello-world` project in *Package Explorer* (if it isn't already).

• From the *File* Menu, select *New > Class*.

• Specify a *Name* of *HelloWorld*. Don't worry about the warning you receive about using the default package. We're just keeping it simple for now. 

*Note: Case here is important. Java classes start with a capital letter and use `camelCase`, capitalizing the first letter of each additional word.*

• Check the box for *public static main void(String[] args)*.

• Click the *Finish* button.

## Now You've Got Class!

You should see code similar to the following in your editor:

```java
public class HelloWorld {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

	}

}
```

# Let's Break It Down

## Java Classes

All Java code is found inside a *class*. This class is called `HelloWorld`.

<pre><code class="language-java" data-noescape>public <mark>class HelloWorld</mark> {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

	}

}
</code></pre>

## Java Methods

Think of *Methods* as the messages that we send in Java. All Java applications start with a `main` method.


<pre><code class="language-java" data-noescape>public class HelloWorld {

	<mark>public static void main(String[] args)</mark> {
		// TODO Auto-generated method stub

	}

}
</code></pre>

## Curly Brackets

Curly brackets (`{` and `}`) indicate code blocks in Java. An opening curly bracket (`{`) must **always, always, always** have a corresponding closing curly bracket (`}`).

### This applies to classes…

% 'data-noescape' attribute tells it to ignore our <mark> tags

<pre><code class="language-java" data-noescape>public class HelloWorld <mark>{</mark>

	public static void main(String[] args) {
		// TODO Auto-generated method stub

	}

<mark>}</mark>
</code></pre>

!SLIDE

### … as well as methods.

<pre><code class="language-java" data-noescape>public class HelloWorld {

	public static void main(String[] args) <mark>{</mark>
		// TODO Auto-generated method stub

	<mark>}</mark>

}
</code></pre>

## Comments

We can add comments to our code to explain it. They don't *do* anything.

Here, Eclipse has created a `TODO` comment for us to remind us that we need to do something—namely, write some code inside the method! We'll do that next.

<pre><code class="language-java" data-noescape>public class HelloWorld {

	public static void main(String[] args) {
		<mark>// TODO Auto-generated method stub</mark>

	}

}
</code></pre>

# Hello World!

A common first program for people to write in a language is a program that says "Hello, World!" That's just what we'll do. Change your code to look like the following:

<pre><code class="language-java" data-noescape>public class HelloWorld {

	public static void main(String[] args) {
		System.out.println("Hello, World!");
	}

}
</code></pre>

`println` is short for "print line". `System.out` represents our console/terminal/command line. Here we are sending a `println` message to `System.out` with the content `"Hello, World!"`

Let's run it, and see what happens!

## A Simple Greeting

Right click inside your editor (the pane where you've been modifying the code), then select *Run As > Java Application*. Your program will run, and your *Console* *view* should display something like the following:

```bash
Hello, World!
```
Climactic, eh?

You've written your first Java program. Congratulations!

## Next Steps

Java is a *strongly-typed* language. The type of `"Hello, World!"` is `String`, which is denoted by the double quotation marks:

<pre><code class="language-java" data-noescape>System.out.println(<mark>"</mark>Hello, World!<mark>"</mark>);</code></pre>

We can also do this with other Strings:

<pre><code class="language-java" data-noescape>System.out.println(<mark>"</mark>I can code it!<mark>"</mark>);</code></pre>

## Other Data Types

We can also display numbers and more complex expressions.

<pre><code class="language-java" data-noescape>System.out.println(42);
System.out.println(1.23);
System.out.println(2 + 3);</code></pre>

Try a few of your own! We'll talk about other data types and expressions in days to come.


% TODO should move this after I've nailed it down

<style type="text/css">
.reveal section img.logo {
	border: none;
	background-color: rgba(255, 255, 255, 0.25);
	padding: 1rem;
}
.reveal ol, .reveal dl, .reveal ul {
	margin: 0 0 1rem 2rem;
}
</style>
