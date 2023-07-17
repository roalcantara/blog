blog

A Simple Blog with Spring Boot and Kotlin

[![MIT license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)][2]
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)][5]
[![Editor Config](https://img.shields.io/badge/Editor%20Config-1.0.1-crimson.svg)][4]
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)][3]
[![Semantic Release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)][9]

## Install

`git clone https://github.com/roalcantara/blog`

### Dependencies

- [git][6]
- [gitlint][7]
- [pre-commit][8]

## Usage

- Run `gradle bootRun` to run the app
- Run `open http://localhost:8080`

## Setup

```sh
brew install gradle maven kotlin
mkdir -p ~/Work/java/blog && cd ~/Work/java/blog
curl https://start.spring.io/starter.zip -d language=kotlin -d type=gradle-project-kotlin -d dependencies=web,mustache,jpa,h2,devtools -d packageName=dev.blog -d name=Blog -o blog.zip
unzip blog.zip
gradle bootRun
gh repo create blog --private --description 'Yet Another Blog App' --disable-wiki --license=MIT --add-readme
git init
git remote add origin git@github.com:roalcantara/blog.git
git branch -M main
git pull --rebase origin main
git commit -am 'chore(bootstrap): Create Spring Boot App'
git push -u origin main
```

## Acknowledgements

- [Standard Readme][5]
- [Conventional Commits][7]
- [Semantic Release][9]
- [Building web applications with Spring Boot and Kotlin][10]

## Contributing

- Bug reports and pull requests are welcome on [GitHub][0]
- Do follow [Editor Config][4] rules.
- Do follow [Git lint][7] rules.
- Everyone interacting in the project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [Contributor Covenant][2] code of conduct.

## License

The project is available as open source under the terms of the [MIT][1] [License](LICENSE)

[0]: https://github.com/roalcantara/blog
[1]: https://opensource.org/licenses/MIT 'Open Source Initiative'
[2]: https://contributor-covenant.org 'A Code of Conduct for Open Source Communities'
[3]: https://conventionalcommits.org 'Conventional Commits'
[4]: https://editorconfig.org 'EditorConfig'
[5]: https://github.com/RichardLitt/standard-readme 'Standard Readme'
[6]: https://git-scm.com 'Git'
[7]: https://jorisroovers.com/gitlint 'git commit message linter'
[8]: https://pre-commit.com 'A framework for managing and maintaining multi-language pre-commit hooks'
[9]: https://semantic-release.gitbook.io/semantic-release 'Semantic Release'
[10]: https://spring.io/guides/tutorials/spring-boot-kotlin 'Building web applications with Spring Boot and Kotlin'
[11]: https://youtu.be/3SNKdr3f9Io 'How to dockerize your Spring Boot API'
