{% if site.data.social.rss or site.theme_settings.rss %}
<li>
    <a feed.xml href="{{ site.data.social.feed.path | default: 'feed.xml' | relative_url }}"
       title="{{ site.data.language.str_rss_follow | default: 'Follow RSS feed' }}">
        </a>
</li>
{% endif %}

{% if site.data.social.email_address or site.theme_settings.email_address %}
<li>
    <a href="mailto:{{ site.data.social.email_address }}"
       title="{{ site.data.language.str_email }}">
		<span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fas fa-envelope fa-stack-1x fa-inverse"></i>
        </span>
    </a>
</li>
{% endif %}


{% assign fb_url = "https://www.facebook.com/" | append: site.data.social.facebook %}
{% assign fb_on = site.data.social.facebook or site.theme_settings.facebook %}
{% include social/icon_partial.html isDisplayed=fb_on url=fb_url social="Facebook" %}

{% assign fk_url = "https://flickr.com/photos/" | append: site.data.social.flickr %}
{% assign fk_on = site.data.social.flickr or site.theme_settings.flickr %}
{% include social/icon_partial.html isDisplayed=fk_on url=fk_url social="Flickr" %}

{% assign ig_url = "https://instagram.com/" | append: site.data.social.instagram %}
{% assign ig_on = site.data.social.instagram or site.theme_settings.instagram %}
{% include social/icon_partial.html isDisplayed=ig_on url=ig_url social="instagram" %}

{% assign se_url = site.data.social.linkedin %}
{% assign se_on = site.data.social.linkedin or site.theme_settings.linkedin %}
{% include social/icon_partial.html isDisplayed=se_on url=se_url social="Linkedin" %}

{% assign pi_url = "https://www.pinterest.com/" | append: site.data.social.pinterest %}
{% assign pi_on = site.data.social.pinterest or site.theme_settings.pinterest %}
{% include social/icon_partial.html isDisplayed=pi_on url=pi_url social="Pinterest" %}

{% assign sc_url = "https://soundcloud.com/" | append: site.data.social.soundcloud %}
{% assign sc_on = site.data.social.soundcloud or site.theme_settings.soundcloud %}
{% include social/icon_partial.html isDisplayed=sc_on url=sc_url social="SoundCloud" %}


{% assign tb_url = "https://" | append: site.data.social.tumblr | append: ".tumblr.com/" %}
{% assign tb_on = site.data.social.tumblr or site.theme_settings.tumblr %}
{% include social/icon_partial.html isDisplayed=tb_on url=tb_url social="Tumblr" %}


{% assign tw_url = "https://twitter.com/" | append: site.data.social.twitter %}
{% assign tw_on = site.data.social.twitter or site.theme_settings.twitter %}
{% include social/icon_partial.html isDisplayed=tw_on url=tw_url social="Twitter" %}


{% assign yt_url = "https://www.youtube.com/channel/" | append: site.data.social.youtube %}
{% assign yt_on = site.data.social.youtube or site.theme_settings.youtube %}
{% include social/icon_partial.html isDisplayed=yt_on url=yt_url social="Youtube" %}
