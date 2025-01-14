using System;
using System.Collections.Generic;
using System.Threading.Tasks;

namespace UixCherryProfile
{
    public class FullStackDeveloper
    {
        public string Name { get; private set; }
        public Dictionary<string, List<string>> TechStack { get; private set; }
        public List<string> PassionateAbout { get; private set; }

        public FullStackDeveloper(string name)
        {
            Name = name;
            TechStack = new Dictionary<string, List<string>>
            {
                { "Frontend", new List<string> { "TypeScript", "React", "Tailwind CSS" } },
                { "Backend", new List<string> { "C#", "ASP.NET Core", "gRPC" } },
                { "Cloud", new List<string> { "Azure", "AWS Lambda", "Docker", "Kubernetes" } },
                { "Databases", new List<string> { "PostgreSQL", "Cosmos DB", "Redis" } }
            };
            PassionateAbout = new List<string> { "Microservices", "CQRS", "Event-Driven Architecture", "DevOps Automation" };
        }

        public async Task SayHiAsync()
        {
            Console.WriteLine($"👋 Hi there, I'm {Name}! 🍒");
            Console.WriteLine("🚀 Let's scale amazing applications together!");
            await SimulateProjectDemoAsync();
        }

        private async Task SimulateProjectDemoAsync()
        {
            Console.WriteLine("\n🌐 Simulating a scalable, event-driven architecture:");
            await Task.Delay(1000); // Simulate processing time
            Console.WriteLine("✅ Microservices deployed with Kubernetes and Docker");
            Console.WriteLine("✅ Real-time data updates handled via SignalR and gRPC");
            Console.WriteLine("✅ Serverless functions running on Azure and AWS");
            Console.WriteLine("\n✨ Ready to build something great together? 🤝");
        }
    }

    class Program
    {
        static async Task Main(string[] args)
        {
            var me = new FullStackDeveloper("uixcherry");
            await me.SayHiAsync();
        }
    }
}
