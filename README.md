import React from 'react';
import { Award, Code, GitBranch, Globe, Terminal, Trophy } from 'lucide-react';

const GithubProfile = () => {
  const techStack = [
    { name: 'HTML5', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg' },
    { name: 'CSS3', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg' },
    { name: 'JavaScript', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg' },
    { name: 'Python', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg' },
    { name: 'Django', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/django/django-plain.svg' },
    { name: 'MySQL', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg' }
  ];

  return (
    <div className="bg-gradient-to-br from-gray-900 to-gray-800 min-h-screen text-white p-8 font-sans">
      <div className="max-w-4xl mx-auto space-y-8">
        {/* Header */}
        <header className="text-center">
          <h1 className="text-4xl font-bold bg-clip-text text-transparent bg-gradient-to-r from-blue-400 to-purple-600 mb-4">
            Hi there, si PJ diay ni! 👋
          </h1>
          <p className="text-gray-300 text-xl max-w-2xl mx-auto">
            A passionate developer continuously learning and building projects with a mission to create innovative solutions.
          </p>
        </header>

        {/* Achievements */}
        <section className="bg-gray-800 rounded-xl p-6 shadow-lg">
          <h2 className="text-2xl font-semibold mb-4 flex items-center">
            <Award className="mr-2 text-yellow-500" /> Achievements
          </h2>
          <div className="grid grid-cols-3 gap-4">
            {[
              '🏔 Arctic Code Vault Contributor',
              '🚀 Mars 2020 Contributor', 
              '💡 Galaxy Brain',
              '🍎 Pair Extraordinaire', 
              '🌟 Starstruck'
            ].map((achievement, index) => (
              <div 
                key={index} 
                className="bg-gray-700 p-3 rounded-lg hover:bg-gray-600 transition-all"
              >
                {achievement}
              </div>
            ))}
          </div>
        </section>

        {/* GitHub Stats */}
        <section className="grid md:grid-cols-3 gap-6">
          <div className="bg-gray-800 rounded-xl p-6 shadow-lg">
            <h3 className="text-xl font-semibold mb-4 flex items-center">
              <GitBranch className="mr-2 text-green-500" /> GitHub Stats
            </h3>
            <img 
              src="https://github-readme-stats.vercel.app/api?username=pjjj23&theme=dark&show_icons=true&bg_color=transparent" 
              alt="GitHub Stats" 
              className="w-full rounded-lg"
            />
          </div>
          <div className="bg-gray-800 rounded-xl p-6 shadow-lg">
            <h3 className="text-xl font-semibold mb-4 flex items-center">
              <Code className="mr-2 text-blue-500" /> Top Languages
            </h3>
            <img 
              src="https://github-readme-stats.vercel.app/api/top-langs/?username=pjjj23&theme=dark&layout=compact&bg_color=transparent" 
              alt="Top Languages" 
              className="w-full rounded-lg"
            />
          </div>
          <div className="bg-gray-800 rounded-xl p-6 shadow-lg">
            <h3 className="text-xl font-semibold mb-4 flex items-center">
              <Terminal className="mr-2 text-purple-500" /> GitHub Streak
            </h3>
            <img 
              src="https://github-readme-streak-stats.herokuapp.com/?user=pjjj23&theme=dark&background=transparent" 
              alt="GitHub Streak" 
              className="w-full rounded-lg"
            />
          </div>
        </section>

        {/* Tech Stack */}
        <section className="bg-gray-800 rounded-xl p-6 shadow-lg">
          <h2 className="text-2xl font-semibold mb-4 flex items-center">
            <Globe className="mr-2 text-cyan-500" /> Tech Stack
          </h2>
          <div className="grid grid-cols-6 gap-4">
            {techStack.map((tech, index) => (
              <div 
                key={index} 
                className="flex flex-col items-center p-4 bg-gray-700 rounded-lg hover:bg-gray-600 transition-all"
              >
                <img 
                  src={tech.icon} 
                  alt={tech.name} 
                  className="w-12 h-12 mb-2"
                />
                <span className="text-sm">{tech.name}</span>
              </div>
            ))}
          </div>
        </section>

        {/* Trophies & Extras */}
        <section className="grid md:grid-cols-2 gap-6">
          <div className="bg-gray-800 rounded-xl p-6 shadow-lg">
            <h2 className="text-2xl font-semibold mb-4 flex items-center">
              <Trophy className="mr-2 text-amber-500" /> GitHub Trophies
            </h2>
            <img 
              src="https://github-profile-trophy.vercel.app/?username=pjjj23&theme=dark&row=1&column=6" 
              alt="GitHub Trophies" 
              className="w-full rounded-lg"
            />
          </div>
          <div className="bg-gray-800 rounded-xl p-6 shadow-lg space-y-4">
            <h2 className="text-2xl font-semibold flex items-center">
              🖤 Fun Extras
            </h2>
            <div className="flex items-center space-x-4">
              <span>Visitor Count:</span>
              <img 
                src="https://visitor-badge.laobi.icu/badge?page_id=pjjj23" 
                alt="Visitor Count" 
              />
            </div>
            <div>
              <span>Random Quote:</span>
              <img 
                src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=dark" 
                alt="Random Quote" 
                className="mt-2"
              />
            </div>
          </div>
        </section>

        {/* Footer */}
        <footer className="text-center text-gray-400 mt-8">
          <p>💬 Feel free to connect, collaborate, or ask me anything about tech. I'm always happy to help!</p>
        </footer>
      </div>
    </div>
  );
};

export default GithubProfile;
