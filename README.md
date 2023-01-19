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

### Commit Message Type
```
👷 build: เมื่อปรับปรุง build config หรือ development tools (เช่น: เกี่ยวข้องกับ npm หรือการเพิ่ม dependencies)
✨ feat: เมื่อเพิ่มคุณสมบัติใหม่ (feature)
🔧 chore: เมื่อมีการเปลี่ยนแปลงค่า Ignore หรือค่า Settings ที่ไม่กระทบกับ Code โดยตรง (เช่นที่: .gitignore หรือ .prettierrc)
🐛 fix: เมื่อแก้ไขข้อผิดพลาด (bug fix)
📝 docs: เมื่อเปลี่ยนแปลงที่เกี่ยวข้องกับเอกสาร
♻️ refactor: เมื่อมีการ Refactor code (เช่น การเปลี่ยนชื่อตัวแปร/ ชื่อฟังก์ชัน)
⚡️ perf: เมื่อทำการเพิ่มประสิทธิภาพ (performance)
💄 style: เมื่อเกี่ยวข้องกับ styling เช่น การจัดรูปแบบใหม่
✅ test: เมื่อเกี่ยวข้องกับการเขียน Testing เพิ่ม หรือ Refactoring tests โดยที่ไม่เกี่ยวข้องกับ Production code
```

[Conventional Commits 1.0.0](https://www.conventionalcommits.org/en/v1.0.0/)