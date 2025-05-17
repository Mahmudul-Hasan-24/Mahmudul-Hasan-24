
# 💫 About Me:
I am pursuing Master´s of Computational Social System (Business Analytics) at University of Graz and Technical University of Graz with skills in Python, data analysis and forecasting. Passionate about business analytics and data-driven development. Actively seeking roles where I can turn data into actionable insights.<br>


## 🌐 Socials:
[![Discord](https://img.shields.io/badge/Discord-%237289DA.svg?logo=discord&logoColor=white)](https://discord.gg/http://discordapp.com/users/1230140416213385266) [![Facebook](https://img.shields.io/badge/Facebook-%231877F2.svg?logo=Facebook&logoColor=white)](https://facebook.com/https://www.facebook.com/share/1AYbsg2LDS/) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/https://www.linkedin.com/in/mahmudul-hasan-764307249?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app) 


# 💻 Tech Stack:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) 
![Anaconda](https://img.shields.io/badge/Anaconda-%2344A833.svg?style=for-the-badge&logo=anaconda&logoColor=white) 
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) 
![Canva](https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=Canva&logoColor=white) 
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) 
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) 
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) 
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) 
![GitLab](https://img.shields.io/badge/gitlab-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white) 
![Jira](https://img.shields.io/badge/jira-%230A0FFF.svg?style=for-the-badge&logo=jira&logoColor=white) 
![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black) 
![Trello](https://img.shields.io/badge/Trello-%23026AA7.svg?style=for-the-badge&logo=Trello&logoColor=white) 
![Excel](https://img.shields.io/badge/MS_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![MiniZinc](https://img.shields.io/badge/MiniZinc-005B94?style=for-the-badge&logo=code&logoColor=white)

# 🛠Skills:

- Problem-solving
- Communication
- Negociation
- Time Management
- Report Writing & Presentation
- Collaboration in Cross-functional Teams
- Data Analysis & Visualization
- Decision-Making


# 📊 GitHub Stats:
![](https://github-readme-stats.vercel.app/api?username=Mahmudul-Hasan&theme=dark&hide_border=false&include_all_commits=false&count_private=false)<br/>
![](https://nirzak-streak-stats.vercel.app/?user=Mahmudul-Hasan&theme=dark&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=Mahmudul-Hasan&theme=dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical)

### 🔝 Top Contributed Repo
![](https://github-contributor-stats.vercel.app/api?username=Mahmudul-Hasan&limit=5&theme=dark&combine_all_yearly_contributions=true)

name: GitHub Snake Game

on:
  # Schedule the workflow to run daily at midnight UTC
  schedule:
    - cron: "0 0 * * *"
  # Allow manual triggering of the workflow
  workflow_dispatch:
  # Trigger the workflow on pushes to the main branch
  push:
    branches:
      - main
jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    steps:
      # Step 1: Checkout the repository
      - name: Checkout Repository
        uses: actions/checkout@v3
      # Step 2: Generate the snake animations
      - name: Generate GitHub Contributions Snake Animations
        uses: Platane/snk@v3
        with:
          # GitHub username to generate the animation for
          github_user_name: ${{ github.repository_owner }}
          # Define the output files and their configurations
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark
            dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
      # Step 3: Deploy the generated files to the 'output' branch
      - name: Deploy to Output Branch
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./dist
          publish_branch: output
          # Optionally, you can set a custom commit message
          commit_message: "Update snake animation [skip ci]"

---
[![](https://visitcount.itsvg.in/api?id=Mahmudul-Hasan&icon=0&color=0)](https://visitcount.itsvg.in)

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
