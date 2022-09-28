<html lang="{{ site.lang | default: "en-US" }}">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">

{% seo %}
    <link rel="stylesheet" href="{{ '/assets/css/style.css?v=' | append: site.github.build_revision | relative_url }}">
    <script src="{{ '/assets/js/scale.fix.js' | relative_url }}"></script>
    <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
    <!--[if lt IE 9]>
    <script src="//html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
  </head>
  <body>
    <div class="wrapper">
      <header>
        <h1 class="header">{{ site.title | default: site.github.repository_name }}</h1>
        <p class="header">{{ site.description | default: site.github.project_tagline }}</p>

        <ul>

	  <li><a class="buttons github" href="https://github.com/jose-tello/TelloEngine/releases/tag/1.0.0">Latest release</a></li>
          <li><a class="buttons github" href="https://github.com/jose-tello/TelloEngine/tree/Usability-improvements">View On GitHub</a></li>
        </ul>

        {% if site.github.is_project_page %}
          <p class="header">This project is maintained by <a class="header name" href="{{ site.github.owner_url }}">{{ site.github.owner_name }}</a></p>
        {% endif %}

        {% if site.github.is_user_page %}
          <ul>
            <li><a class="buttons github" href="{{ site.github.owner_url }}">GitHub Profile</a></li>
          </ul>
        {% endif %}
      </header>

      <section>
        {{ content }}
      </section>

      <footer>
        <p><small>Hosted on <a href="https://pages.github.com">GitHub Pages</a> using the Dinky theme</small></p>
      </footer>
    </div>
    <!--[if !IE]><script>fixScale(document);</script><![endif]-->
    {% if site.google_analytics %}
      <script>
        (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
        (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
        m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
        })(window,document,'script','//www.google-analytics.com/analytics.js','ga');
        ga('create', '{{ site.google_analytics }}', 'auto');
        ga('send', 'pageview');
      </script>
    {% endif %}
  </body>
</html>
