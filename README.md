👋 Hi there, I'm uixcherry 🍒

```typescript
class FullStackDeveloper {
  constructor(name: string) {
    this.name = name;
    this.techStack = {
      frontend: ["TypeScript", "JavaScript", "React"],
      backend: ["C#", ".NET", "ASP.NET"],
      databases: ["MongoDB", "SQLite", "SQL Server"]
    };
    this.passionateAbout = ["clean code", "SOLID principles", "best practices"];
  }

  sayHi() {
    console.log(`Let's build something great together, ${this.name} 🤝`);
  }
}

const me = new FullStackDeveloper("uixcherry");
me.sayHi();
