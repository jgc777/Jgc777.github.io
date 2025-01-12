👋 Hi, I'm *Jgc7*.
- 💬 Ask me about Windows, Minecraft, Scratch, C#, Kali Linux, video editing, maths...
- 📫 How to reach me: [jgc-7@outlook.com](mailto:jgc-7@outlook.com) or [discord](http://discord.com/users/889045882874495036)
- You can see more in my [gravatar](https://gravatar.com/jgc9884) or my [YouTube](https://www.youtube.com/channel/UCCfLGV3QvExntjvWGbPjOUQ?sub_confirmation=1).
- My public projects:

<ul id="repo-list"></ul>
<script>
  const username = "jgc777";
  async function fetchRepos() {
    try {
      const response = await fetch(`https://api.github.com/users/${username}/repos`);
      if (!response.ok) {
        throw new Error("Error obtaining repos");
      }
      const repos = await response.json();
      const repoList = document.getElementById("repo-list");
      repos.forEach(repo => {
        const repoNameLower = repo.name.toLowerCase();
        const usernameLower = username.toLowerCase();
        if (repoNameLower === usernameLower || repoNameLower === `${usernameLower}.github.io`) {
          return;
        }
        const listItem = document.createElement("li");
        const link = document.createElement("a");
        const pagesUrl = `https://${username}.github.io/${repo.name}`;
        link.href = repo.has_pages ? pagesUrl : repo.html_url; // Priorizar GitHub Pages
        link.textContent = repo.name;
        listItem.appendChild(link);
        repoList.appendChild(listItem);
      });
    } catch (error) {
      console.error(error);
    }
  }
  fetchRepos();
</script>


[![Discord](https://discord-readme-badge.vercel.app/api?id=889045882874495036)](https://discord-readme-badge.vercel.app/api?id=889045882874495036)
