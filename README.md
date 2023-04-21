![iankaguer's GitHub stats](https://github-readme-stats.vercel.app/api?username=iankaguer&show_icons=true&theme=tokyonight)
![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=DenverCoder1)
![](https://komarev.com/ghpvc/?username=iankaguer)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=iankaguer&show_icons=true&theme=tokyonight&layout=compact)
![iankaguer's wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=iankaguer&theme=tokyonight)


name: Waka Readme

on:
  schedule:
    # Runs at 12am IST
    - cron: '30 18 * * *'
  workflow_dispatch:
jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}


