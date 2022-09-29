# Contributing to Tenacom projects

Thanks for taking the time to contribute to one (or even more) of our open-source projects!

The following is a set of guidelines for contributing to any project hosted in the [Tenacom](https://github.com/Tenacom) organization on GitHub. Feel free to propose changes to this document by opening an issue on our [Community Health project](https://github.com/Tenacom/.github).

> **NOTE:** If you just want to ask a question, please use the Discussions area of the relevant repository.

- [Code of Conduct](#code-of-conduct)
- [What should I know before I get started?](#what-should-i-know-before-i-get-started)
  - [Who we are](#who-we-are)
    - [Why open source?](#why-open-source)
    - [Our philosophy](#our-philosophy)
  - [Legal stuff](#legal-stuff)
    - [About licensing](#about-licensing)
    - [About copyright](#about-copyright)
    - [Author identification](#author-identification)
- [How can I contribute?](#how-can-i-contribute)
  - [Reporting bugs](#reporting-bugs)
  - [Suggesting enhancements](#suggesting-enhancements)
  - [Contributing code](#contributing-code)
    - [Where to begin](#where-to-begin)
    - [Setting up for local development](#setting-up-for-local-development)
    - [Working on a Tenacom project](#working-on-a-tenacom-project)
    - [Pull requests](#pull-requests)
- [Style guides](#style-guides)
  - [Git commit message style guide](#git-commit-message-style-guide)
  - [C# code style guide](#c-code-style-guide)
    - [Advanced topics](#advanced-topics)
    - [Source files and their names](#source-files-and-their-names)
  - [XML documentation style guide](#xml-documentation-style-guide)
  - [Unit test style guide](#unit-test-style-guide)
  - [XML (project files, MSBuild files) style guide](#xml-project-files-msbuild-files-style-guide)

## Code of Conduct

Tenacom projects and everyone participating in them are governed by the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [community@tenacom.it](mailto:community@tenacom.it).

## What should I know before I get started?

### Who we are

Tenacom is a very small software house with very big ideas, :grin: founded in 2015 by Riccardo De Agostini a.k.a. [@rdeago](https://github.com/rdeago). We are located in North-Eastern Italy.

Our main source of revenue is smart interfaces (think microservices, but nicely packaged as tiny embedded computers) that add networking and automation capabilities to traditional field devices. Instead of having to deal with proprietary protocols over serial ports, we enable applications to integrate devices using simple, standard protocols based on e.g. TCP, HTTP, and WebSockets.

You will hardly find out about us on the Web. In fact, we don't even have a site: our reputation is built exclusively on word of mouth between customers and prospects. Even so, we often have to decline requests for custom projects because of lack of time.

#### Why open source?

Just like every other software house on Earth, we wouldn't even be in business if it wasn't for open-source software. Unlike the great majority of them, though, we openly admit it. Releasing some of our internal libraries and tools as open-source projects is our way to give back at least some of what we received.

#### Our philosophy

We believe in software development as a form of artisanship, where every individual contribution is valued.

We strive to follow best practices, sometimes adapting them to our small-team reality.

Although we are constantly looking into any way to improve our procedures, code quality and customer satisfaction mean a lot more to us than any trend or buzzword. To clarify for Agile fanboys: we don't "do Agile", we _are_ agile.

### Legal stuff

#### About licensing

We do not require contributors to sign any particular agreement ([CLA](https://en.wikipedia.org/wiki/Contributor_License_Agreement), [DCO](https://en.wikipedia.org/wiki/Developer_Certificate_of_Origin), or otherwise) in order to accept their submissions.

This means that, as stated in [GitHub's Terms of Service, section D-6](https://docs.github.com/en/site-policy/github-terms/github-terms-of-service#6-contributions-under-repository-license), by submitting your contributions you will implicitly agree to license them to us under the same agreement (usually the [MIT License](https://choosealicense.com/licenses/mit/)) under which the project is released to the public. This principle is called "inbound = outbound" and is traditionally implied, but GitHub cleverly wrote it down to avoid misunderstandings.

#### About copyright

To quote [GitHub's Terms of Service, section D-3](https://docs.github.com/en/site-policy/github-terms/github-terms-of-service#3-ownership-of-content-right-to-post-and-license-grants):

> You retain ownership of and responsibility for Your Content. If you're posting anything you did not create yourself or do not own the rights to, you agree that you are responsible for any Content you post; that you will only submit Content that you have the right to post; and that you will fully comply with any third party licenses relating to Content you post.

In order to accept a submission containing code and/or other content that is not the original work of the contributor (for example, a small utility method copied from a third-party open-source library to avoid taking an extra dependency), we require that:

- the original author is identified (for example by putting a link to the original content in a comment), and
- the `THIRD-PARTY-NOTICES` file in the repository root is updated with the relevant attribution, if so required by the license of the original content (although attribution is never forbidden, so it is a good idea to add it as a principle.)

#### Author identification

When we use the collective term "contributors" (for example in the text of our license agreements) we mean <u>commit authors</u>, as publicly visible in each repository's commit history.

## How can I contribute?

### Reporting bugs

This section guides you through submitting a bug report for a Tenacom project. Following these guidelines helps maintainers and the community understand your report, reproduce the behavior, and find related reports.

Before creating a bug report, please take the time to **search in the Issues area** of the project to see if the problem has already been reported. If it has **and the issue is still open**, add a comment to the existing issue instead of opening a new one. If you are unsure, post a question in the Discussions area of the project.

When you are creating a bug report, please **use a clear and descriptive title** for the issue nd fill out the required template including **as many details as possible**: any little piece of information could be decisive in resolving the issue.

> **Note:** If you find a **Closed** issue that seems like it is the same thing that you're experiencing, open a new issue and include a link to the original issue in the body of your new one.

### Suggesting enhancements

This section guides you through submitting an enhancement suggestion for a Tenacom project, including completely new features and minor improvements to existing functionality. Following these guidelines helps maintainers and the community understand your suggestion and find related suggestions.

Before creating enhancement suggestions, please take the time to **search in the Issues area** of the project to see if the enhancement has already been suggested. If it has, add a comment to the existing issue instead of opening a new one.

When you are creating an enhancement suggestion, please **use a clear and descriptive title** for the issue and fill out the required template including **as many details as possible**.

### Contributing code

#### Where to begin

Unsure where to begin contributing code to a Tenacom project? You can start by looking through `easy` and `help-wanted` issues:

- Issues with an `easy` label should only require a few lines of code, and a test or two.
- Issues with a `help-wamted` label are usually more involved than `easy` issues.

#### Setting up for local development

We strive to make onboarding as straightforward as possible. Unless otherwise specified in a project's `README.md`, all it takes to start tinkering with a Tenacom project is an up-to-date Community edition of Microsoft Visual Studio.

Just fork the project you want to work on, create a new branch from `main` (for enhancements) or from the most recent `vN.N` branch (for bug fixes), and start coding. If you are unsure about how to proceed, GitHub has a detailed guide on [working with forks](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/about-forks) that explains more, and better, than I ever could.

#### Working on a Tenacom project

Open-source projects are usually teamwork. Teams have rules, and Tenacom is no exception. Just as we respect and value every contributor's work and the time put into it, we ask for the same respect towards the work and time of others. Style guides and technical rules exist for exactly this purpose.

> Always code as if the guy who ends up maintaining your code will be a violent psychopath who knows where you live. Code for readability.
> _- [John F. Woods](https://groups.google.com/g/comp.lang.c++/c/rYCO5yn4lXw/m/oITtSkZOtoUJ)_

Some quick "do"s and "don't"s:

- DO follow the [Style guides](#style-guides), both when coding and when writing [commit messages](#git-commit-message-style-guide).
- Do keep an eye on Visual Studio's [Error List window](https://learn.microsoft.com/en-us/visualstudio/ide/reference/error-list-window) and let static code analyzers guide you.
- DO maintain style consistent with adjacent code (same file > same folder > same project) when in doubt
- DO use latest C# features liberally, as long as code readability is not negatively affected.
- DO write XML documentation for everything you add, and keep it up to date for everything you modify.
- DO write unit tests for every feature you add, and regression tests for every bug you fix.
- DO NOT modify `.editorconfig`, `.globalconfig`, `stylecop.json`, etc. to suit _your_ coding style, because then _all other code_ will trigger warnings. Also, we're not interested in PRs that globally change code style.
- DO remember that _any_ warning (including code-style-related warnings) will prevent a pull request from passing automatic checks. If you think I'm just being a control freak, try finding a potential null-reference return in your code among 700 leftover warnings.
- DO NOT use Visual Studio's "Project Properties" window. Instead, manually maintain project files. Do you like it when you can understand how a project is built, what it contains and what it doesn't, how the build is configured? I thought so. So does other people.
- DO check for Visual Studio's automatic modifications to project files before staging them; verify that they make actual sense.
- DO follow the [style guide for Git commit messages](#git-commit-message-style-guide).
- DO make small and consistent commits. Notice a typo in the XML docs of a method you were otherwise not touching? Thanks for the fix, but that's _a separate commit_.
- DO keep `PublicAPI.Unshipped.txt` files up to date.
- DO NOT modify `PublicAPI.Shipped.txt` files, as they are maintained automatically.

#### Pull requests

When you think your code is ready, open a pull request on the relevant repository, following all instructions in [the pull request template](.github/PULL_REQUEST_TEMPLATE.md). One of the project maintainers will review it, maybe as for some modifications, and finally approve it.

Every pull request must pass some status checks before being merged into the project. At the minimum, the project must build with no errors (and no warnings - did you follow the style guides?) and all tests must pass. A reviewer may ask you to complete additional work before accepting your pull request: for example, add one or more tests, update public API files, 

## Style guides

### Git commit message style guide

- Use the present tense ("_Add_ foobars", not "_Added_ foobars" or "_Adding_ foobars".)
- Use the imperative mood ("_Add_ foo to bar", not "_Adds_ foo to bar".)
- Limit the first line to 72 characters or less.
- Do not terminate the first line with punctuation ("Add foobars", not "Add foobars.")
- Optionally use the lines after the first to better illustrate what you did; here you can also refer to issues or other PRs using the hash syntax (#123 to mean issue or PR number 123.)
- Do not use any particular prefix (e.g. `[FIX]`, `fix:`, etc.)
- You can [sign off](https://github.com/git/git/blob/master/Documentation/signoff-option.txt) your commits if you want, but it is not a requirement.

### C# code style guide

All our projects include `.editorconfig` and `.globalconfig` files, as well as pre-configured static code analyzers that will check your coding style in real time.

#### Advanced topics

Some quick "do"s and "don't"s about stuff that code analyzers won't catch (reviewers, though, will):

- DO NOT disable warnings unless absolutely necessary. Even then, explain the reason in a comment, and restore the warning(s) immediately afterwards.

  ```C#
  #pragma warning disable CA2012 // Use ValueTasks correctly - This is correct usage, because we consume the ValueTask only once.
      public void Dispose() => DisposeAsync().ConfigureAwait(false).GetAwaiter().GetResult();
  #pragma warning restore CA2012 // Use ValueTasks correctly
  ```

- DO always use `@this` as the first parameter name of extension methods:

  ```C#
    public static void Rethrow(this Exception @this) => ExceptionDispatchInfo.Throw(@this);
  ```

- DO only use the English language for identifier names. Prefer American spelling, e.g. `color` instead of `colour` ([more examples of spelling differences](https://www.oxfordinternationalenglish.com/differences-in-british-and-american-spelling/)).
- DO only use the English language in comments. Please write in [plain English](http://www.plainenglish.co.uk/how-to-write-in-plain-english.html) as much as you can: we are not all native speakers.

#### Source files and their names

- Put exactly one type in each file. Yes, even enums. Yes, even delegates. This makes looking for a type very easy, even outside an IDE.
- File name must be the name of the first (and only) contained type.
  - For generic types, append a grave accent `` ` `` followed by the type's arity (the number of type parameters). Example: `MagicalConverter<TInput, TOutput>` has two type parameters, hence the file name will be ``MagicalConverter`2.cs``.
  - For nested types, use the name of the containing type, followed by a dot `.` and the name of the nested type. Example: `struct MyClass.PrivateData` goes in `MyClass.PrivateData.cs`.
  - Extension methods should be grouped in extension classes (static classes that only contain extension methods) whose name is the name of the type being extended, followed by `Extensions`. For example: file `FooExtensions.cs` contains the `FooExtensions` static class, whose methods are extension methods for objects of type `Foo`.
  - Names of extensions classes for interfaces must not start with `I`. For example: file `FooExtensions.cs` contains the `FooExtensions` static class, whose methods are extension methods for objects that implement interface `IFoo`.
- When you split a type across multiple files (`partial` type), always have a file named after the type, where you put the XML documentation for the type and the full type declaration. In other files, group members either by name (for example if there are a dozen overloads of the same method `FooExtensions.Bar`, it makes sense to put them in their own file) or by topic. For example, let's pretend we wrote an extension class for `DateTime`, with methods like `GetNextMonday()` (gets the Monday after a `DateTime`) and `AddHalfSeconds` (adds _half_ the specified number of seconds to a `DateTime`):

  ```C#
  // DateTimeExtensions.cs
  using System;
  
  namespace MyLib;
  
  /// <summary>
  /// Provides extension methods for instances of <see cref="DateTime"/>.
  /// </summary>
  [VeryUseful]                                   // <--- Type attributes go here
  public static partial class DateTimeExtensions // <--- Full type modifiers here
  {
  }
  ```

  ```C#
  // DateTimeExtensions-daysOfWeek.cs   <--- Methods grouped by topic - notice the small "d" after the minus sign
  using System;
  
  namespace MyLib;
  
  partial class DateTimeExtensions // <--- ONLY "partial" here
  {
    // Methods GetNextMonday(), GetNextTuesday(), etc. go here.
  }
  ```

  ```C#
  // DateTimeExtensions-AddHalfSeconds.cs   <--- Overloads of the same method - notice the method name after the minus sign
  using System;
  
  namespace MyLib;
  
  partial class DateTimeExtensions // <--- ONLY "partial" here
  {
    // Methods AddHalfSeconds(int), AddHalfSeconds(long), AddHalfSeconds(double) go here.
  }
  ```

### XML documentation style guide

**TODO**

### Unit test style guide

**TODO**

### XML (project files, MSBuild files) style guide

**TODO**
