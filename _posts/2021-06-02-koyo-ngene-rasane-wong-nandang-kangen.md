---
layout: post
title: Koyo Ngene Rasane Wong Nandang Kangen
feature-img: "assets/img/feature-img/desk-messy.jpeg"
thumbnail: "assets/img/thumbnails/feature-img/desk-messy.jpeg"
tags: [Kangen, Wong]
---
* TOC
{:toc}
Kangen iku ancen e angel tombone,Koyok lirik lagune wong sing jenenge nella:

```yaml
feature-img: "assets/img/feature-img/desk-messy.jpeg"
thumbnail: "assets/img/thumbnails/feature-img/desk-messy.jpeg" 
```

Kangen dapat mengacu pada beberapa hal berikut: Perasaan, perasaan rindu yang mendalam kepada seseorang atau sesuatu yang sudah lama tidak ditemui.
Kangen kui iso mengacu karo Roso ning ati, Roso Rindu sing njero nggo uwong sing wis suwe ra tau ketemu.


>  - Koyo Ngene Rasane Kangen

Kamu bisa menerka nerka apa sih yang dirasain oleh orang yang kamu kangen in. Tapi alangkah baiknya kalau kamu mengungkapkannya. `Kangen` include.
Make sure to separate all of thePastikan perasaanmu kui kangen beneran. Dudu Guyonan. Soale kangen e wong iku wes angel tombone kecuali ketemu. `,`.
It by default look into `assets/img/` so give the path from there, example:

{% highlight ruby %}
{% raw %}
{% include aligner.html images="pexels/book-glass.jpeg,triangle.png" %}
{% endraw %}
{% endhighlight %}

{% include aligner.html images="pexels/book-glass.jpeg,feature-img/desk-messy.jpeg" %}


Here you have two images side by side, but you can set more and set the amount per columns 
(by specifying the number of columns or let it be automatic using `"auto"`):

{% highlight ruby %}
{% raw %}
{% include aligner.html images="portfolio/cabin.png,portfolio/cake.png,portfolio/circus.png" column=3 %}
{% endraw %}
{% endhighlight %}

{% include aligner.html images="portfolio/cabin.png,portfolio/cake.png,portfolio/circus.png" column=3 %}

it also works with only one images, it is made to display it smaller than normally.
However you can just use the Markdown way of doing it to get the image normal sized and centered.

{% highlight ruby %}
{% raw %}
# Markdown way (bigger)
![Travel]({{ "/assets/img/pexels/computer.jpeg" | relative_url}})
# Aligner with only One (50% of width)
{% include aligner.html images="pexels/computer.jpeg" %}
{% endraw %}
{% endhighlight %}

{% include aligner.html images="pexels/computer.jpeg" %}
