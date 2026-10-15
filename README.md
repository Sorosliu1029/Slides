# Slides

Talks by Soros Liu, built with [reveal.js](https://revealjs.com).

👉 https://slides.sorosliu.xyz/

| Date       | Talk                                                                   | Source                                                       |
| ---------- | ---------------------------------------------------------------------- | ------------------------------------------------------------ |
| 2021-10-25 | [Explore Git](https://explore-git.sorosliu.xyz/mock.slides.html)        | [`explore-git/`](https://github.com/Sorosliu1029/Explore-Git) (submodule) |
| 2021-09-06 | [B+ Tree](https://slides.sorosliu.xyz/b-tree/)                          | [`b-tree/`](b-tree/)                                         |
| 2019-04-14 | [Redis 持久化](https://slides.sorosliu.xyz/redis-persistence/)          | [`redis-persistence/`](redis-persistence/)                   |
| 2018-11-26 | [如何赚xxd的红包 - 台球篇](https://slides.sorosliu.xyz/billiards/)      | [`billiards/`](billiards/)                                   |

## Layout

```
index.html            # landing page listing every talk
CNAME                 # custom domain for GitHub Pages
explore-git/          # git submodule: Sorosliu1029/Explore-Git
<talk>/               # one self-contained folder per talk
  index.html          #   the slides
  css/ js/ lib/ plugin/  # the reveal.js files this talk uses
  images/             #   the talk's own images
```

Each talk folder carries its own copy of reveal.js and loads nothing from the
other folders, so a talk can be opened, moved or removed on its own.
Explore Git is a Jupyter notebook talk that lives in its own repository and
publishes its slides to https://explore-git.sorosliu.xyz/. It is included here
as a git submodule; clone with `--recurse-submodules`, or run
`git submodule update --init` in an existing clone. To move it to the latest
commit, run `git submodule update --remote explore-git` and commit the change.

## Adding a talk

1. Copy an existing talk folder, e.g. `cp -R redis-persistence my-talk`.
2. Replace the slides in `my-talk/index.html` and put images in `my-talk/images/`.
3. Add an entry to `index.html` and to the table above.

## Preview locally

```sh
python3 -m http.server 8000
# open http://localhost:8000/
```
