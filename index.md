<style>
  header {
    border-bottom: none;
    padding-bottom: 0;
  }
</style>

![Tree from Blade Runner 2049](https://files.jordanreger.com/bladerunner2049tree.jpg)

I am a generalist software engineer from Columbus, Ohio trying to write simple software. I am [AWS](https://files.jordanreger.com/aws_cloud_practitioner_certificate.pdf) and [NWS](https://files.jordanreger.com/advanced_skywarn_certificate.png) cloud certified. I also like riding bikes, making coffee, chasing storms, minimalism, philosophy, languages, cameras, urban planning, and a lot of other things.

---

## Documents

<div id="list"></div>
<script>
  (async () => {
    const response = await fetch('https://api.github.com/repos/jordanreger/doc/contents/');
    const data = await response.json();
    let htmlString = '<ul>';
        
    for (let file of data) {
      if (file.name === ".gitattributes" || file.name === "_config.yml" || file.name === "index.md") {
        continue;
      }
      htmlString += `<li><a href="./doc/${file.path.replace(".md", "")}">${file.name.replace(".md", "")}</a></li>`;
    }

    htmlString += '</ul>';
    document.getElementById('list').innerHTML = htmlString;
  })()
</script>

---

## Projects

### NWS bots

Source: [jordanreger/wx](https://github.com/jordanreger/wx)

Homepage: [jordanreger.github.io/wx](/wx)

Written in Go. Together, bots have ~400 followers on Bluesky. Runs every 15 seconds.

### HTMLsky

Source: [jordanreger/htmlsky](https://github.com/jordanreger/htmlsky)

Homepage: [htmlsky.app](https://htmlsky.app)

Server-side rendered, HTML-only Bluesky frontend.

### More...

You can view my unmaintained software on [Sourcehut](https://sr.ht/~jordanreger) and on [GitHub](https://github.com/jordanreger).
