# 🎉 DEMO Auto Changelog
A commit message auto changelog is a tool that automatically generates a summary of changes made in a code repository based on the commit messages. It helps to keep track of updates and improvements made to the codebase.

### Quick Start
```
npm install -g standard-changelog
```

### Yarn Initial
```
yarn init -y
```

### Conventional Changelog
```
standard-version
```

### Commit Message Structure
```
<type>[optional scope]: <subject>

[optional body]

[optional footer(s)]
```

### Commit Message Type
- 📦 build: เมื่อปรับปรุง build config หรือ development tools (เช่น: เกี่ยวข้องกับ npm หรือการเพิ่ม dependencies)
- ✨ feat: เมื่อเพิ่มคุณสมบัติใหม่ (feature)
- 💧 chore: เมื่อมีการเปลี่ยนแปลงค่า Ignore หรือค่า Settings ที่ไม่กระทบกับ Code โดยตรง (เช่นที่: .gitignore หรือ .prettierrc)
- 🐛 fix: เมื่อแก้ไขข้อผิดพลาด (bug fix)
- 📚 docs: เมื่อเปลี่ยนแปลงที่เกี่ยวข้องกับเอกสาร
- ♻️ refactor: เมื่อมีการ Refactor code (เช่น การเปลี่ยนชื่อตัวแปร/ ชื่อฟังก์ชัน)
- ⚡️ perf: เมื่อทำการเพิ่มประสิทธิภาพ (performance)
- 🍺 style: เมื่อเกี่ยวข้องกับ styling เช่น การจัดรูปแบบใหม่
- 🙏 test: เมื่อเกี่ยวข้องกับการเขียน Testing เพิ่ม หรือ Refactoring tests โดยที่ไม่เกี่ยวข้องกับ Production code

# Example

#### build
```
build(npm): update fsevents to 1.0.14 (#11686)
build(tsc-wrapped): use tsickleCompilerHost for initial file Load
build(docs-infra): enable ServiceWorker in cli config (#25997)
build(common): don't generate .d.ts & .metadata.json files for 118n locales
build(aio): run the upload server as a non-previleged user
build(gulp): use gulp-watch instead of gulp.watch for watching files
build(docs-infra): upgrade webpack-cli to 3.1.2 (#26202)
```

#### docs
```
docs(changelog): update change log to rc.5
docs(zone.js): update DEVELOPER.md for changelog instruction (#32016)
docs(core): fix API docs for ContentChild and ViewChildren (#13656)
docs(MockConnection) add mockError usage example (#8888)
docs(router): clarify scroll position wording (#25077)
docs(readme): remove incorrect download count badge
docs(aio): fix typo (#20193)
docs(router): improve docs for Instruction and related classes
```

#### feat
```
feat(zone.js): support Promise.allSettled (#31849)
feat(ivy): resolve references to vars in .d.ts files (#25775)
feat(aio): implement `GithubTeams`
feat(facade): add bool type
featCforms): add NgForm method that resets submit state (#10715)
feat(parser): improve error handling
feat(bazel): add additional parameters to `ts_api_guardian_test` def (#25694)
```

#### fix
```
fix(ivy): correctly resolve shorthand property declarations (#28936)
fix(bazel): incorrectly always uses ngc-wrapped from "npm" workspace (#28137)
fix(di): injecting null causes a cyclic dependency
fix(ivy): not throwing error for unknown properties on container nodes (#29691)
fix(router): make router provides work with cli and offline compilation
fix(ivy): missing schematics field in localize package (#33025)
fix(forms): avoid producing an error with hostBindingTypeCheck
```

#### perf
```
perf(ivy): don't store public input names in two places (#33798)
perf(ivy): split hooks processing into init and check phases (#32131)
perf(ivy): remove check for function type in renderStringify (#30838)
perf(ivy): removes generation of comments (#21638)
perf(change detection): minimized amount of code in protective try-catch
perf(docs-infra): avoid unnecessary I/0 operation in `ng-packages-installer` (#28510)
perf(dom): only send values for existing properties to js interior
perf(core): make `PlatformLocation` tree-shakable (#32154)
```

#### refactor
```
refactor(compiler): rename decorator directives into directive
refactor(ivy): remove need for LContainer.template (#24335)
refactor(DirectiveResolver): cleanup
refactor(forms): remove facade (#12558)
refactor(core): remove deprecated `bootstrap` (#10831)
refactor(ShadowCss): cleanup
refactor(core): simplify & cleanup reflection
```

#### style
```
style(aio): add space between `.home` and `.hamburger` (#23624)
style(bazel): fix 2 unformatted `.bzl` files
style(core): fix max line Length to pass Linting (#20441)
style(nodeTree): fix formatting
style(compiler): fix Lint issues (#23480)
style(aio): fix indentation on location service spec
style(changelog): improving readability (#18949) PR Close #18949
style(playground): use single quotes consistently
```

#### test
```
test(common): add PercentPipe round and trim tests (#27365)
test(compiler-cli): add test for missingTranslation parameter
test(upgrade): re-enable tests that have been fixed (#27305)
test(ivy): update root causes for @angular/core TestBed failures (#27650)
test(docs-infra): fix tests (#26202)
test(ivy): add attribute interpolation test (#30503)
test(ivy): add canonical compiler spec for class/style (#22719)
test(ivy): mark jit_summaries_integration_spec as obsolete in Ivy (#28027)
test(ivy): split out provider tests (#27069)
```

[Conventional Commits 1.0.0](https://www.conventionalcommits.org/en/v1.0.0/)
