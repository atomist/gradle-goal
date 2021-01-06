# `atomist/gradle-goal`

An Atomist goal to run Gradle phase from an Software Delivery Machine (SDM).

## Usage

### Gradle `assemble`

Put the following YAML into your SDM goal definition to use the `assemble`
task.

```yaml
gradle_build:
  
  goals:
  - atomist/gradle-goal/assemble@master
      parameters:
        options: <optional Gradle options to pass>
        tag: <optional Gradle Docker image tag to use>
```       

### Custom Gradle task

If you want to create a custom Gradle goal that executes a different task, use the following definition

```yaml
gradle_build:
  
  goals:
  - atomist/gradle-goal/gradle-6-jdk-8@master
      parameters:
        task: <Gradle task, by default assemble>
        options: <optional Gradle options to pass>
        tag: <optional Gradle Docker image tag to use>
```    

## Getting started

See the [Developer Quick Start][atomist-quick] to jump straight to
creating an SDM.

[atomist-quick]: https://docs.atomist.com/quick-start/ (Atomist - Developer Quick Start)

## Contributing

Contributions to this project from community members are encouraged
and appreciated. Please review the [Contributing
Guidelines](CONTRIBUTING.md) for more information. Also see the
[Development](#development) section in this document.

## Code of conduct

This project is governed by the [Code of
Conduct](CODE_OF_CONDUCT.md). You are expected to act in accordance
with this code by participating. Please report any unacceptable
behavior to code-of-conduct@atomist.com.

## Documentation

Please see [docs.atomist.com][atomist-doc] for
[developer][atomist-doc-sdm] documentation.

[atomist-doc-sdm]: https://docs.atomist.com/developer/sdm/ (Atomist Documentation - SDM Developer)

## Connect

Follow [@atomist][atomist-twitter] and [The Composition][atomist-blog]
blog related to SDM.

[atomist-twitter]: https://twitter.com/atomist (Atomist on Twitter)
[atomist-blog]: https://the-composition.com/ (The Composition - The Official Atomist Blog)

## Support

General support questions should be discussed in the `#help`
channel in the [Atomist community Slack workspace][slack].

If you find a problem, please create an [issue][].

[issue]: https://github.com/atomist/npm-goal/issues

---

Created by [Atomist][atomist].
Need Help?  [Join our Slack workspace][slack].

[atomist]: https://atomist.com/ (Atomist - How Teams Deliver Software)
[slack]: https://join.atomist.com/ (Atomist Community Slack)
