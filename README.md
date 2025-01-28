```ts
const clientSkills = [
  { language: 'HTML5', icon: '📄' },
  { language: 'CSS3', icon: '🖌️' },
  { language: 'JavaScript', icon: '🧠' },
];

const serverDatabaseSkills = [
  { technology: 'Node.js', icon: '🔗' },
  { technology: 'MongoDB', icon: '🍃' },
];

const frameworksLibs = [
  { framework: 'React / Next.js', icon: '⚛️' },
  { framework: 'TailwindCSS', icon: '🎨' },
];

const studying = [
  { technology: 'Electron', icon: '🖥️' },
  { technology: 'React Native', icon: '📲' },
];

const getSkills = (skills: Array<{ language?: string; technology?: string; framework?: string; icon: string }>) => {
  return skills.map((skill, index) => `${skill.icon} ${skill.language || skill.technology || skill.framework}`);
};

console.log('Client:', getSkills(clientSkills).join('\n'));
console.log('Server & Database:', getSkills(serverDatabaseSkills).join('\n'));
console.log('Frameworks/Libs:', getSkills(frameworksLibs).join('\n'));
console.log('Studying:', getSkills(studying).join('\n'));
```
