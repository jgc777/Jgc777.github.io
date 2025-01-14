👋 Hi, I'm *Jgc7*.
- 💬 Ask me about Windows, Minecraft, Scratch, C#, Kali Linux, video editing, maths...
- 📫 How to reach me: [jgc-7@outlook.com](mailto:jgc-7@outlook.com) or [discord](http://discord.com/users/889045882874495036)
- You can see more in my [gravatar](https://gravatar.com/jgc9884) or my [YouTube](https://www.youtube.com/channel/UCCfLGV3QvExntjvWGbPjOUQ?sub_confirmation=1).
- These are my public projects:

<ul style="list-style: none;"><li><ul id="repo-list" style="list-style: disc;"></ul></li></ul>async function fetchRepos(username, repoList) {repoList.innerHTML = '';if (username === "") {const errorElement = document.createElement("a");errorElement.innerHTML = "No username given!";repoList.appendChild(errorElement);return;}const response = await fetch(`https://api.github.com/users/${username}/repos`);if (!response.ok) {const errorElement = document.createElement("a");errorElement.innerHTML = "Error obtaining repos";repoList.appendChild(errorElement);return;}const repos = await response.json();repos.forEach(repo => {const repoNameLower = repo.name.toLowerCase();const usernameLower = username.toLowerCase();if (repoNameLower === usernameLower || repoNameLower === `${usernameLower}.github.io`) return;const listItem = document.createElement("li");const link = document.createElement("a");const pagesUrl = `https://${username}.github.io/${repo.name}`;link.href = repo.has_pages ? pagesUrl : repo.html_url;link.textContent = repo.name;listItem.appendChild(link);repoList.appendChild(listItem);});}</script><script>fetchrepos("jgc777", document.getElementById('repo-list'))</script>

- This is my Discord status:

<div align="center"><img  src="https://discord-readme-badge.vercel.app/api?id=889045882874495036" width="300px" alt="discord status" style="border-radius: 10px; margin: 20px 0; box-shadow: 0 8px 30px rgba(0, 0, 0, 0.12);"></div>
