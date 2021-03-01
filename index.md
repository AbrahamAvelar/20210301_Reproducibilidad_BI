  
    
          Introducción a reproducibilidad en bioinformática
![langebio](images/langebio.png)  

En este curso aprenderás herramientas de control de versiones, Git y OpenRefine que facilitan la reproducibilidad en análisis de datos. También revisaremos buenas prácticas en organización de archivos y tablas con datos para biología.  

## Calendario  
|        Lunes 1 de Marzo         |
|---------------------------------|
|  ["Tipos" de bioinformáticos](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003496)  |
|[Reglas básicas de Reproducibilidad](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003285)|
| [Data Organization for Ecology](https://datacarpentry.org/spreadsheet-ecology-lesson/)  |
| [Project Management for genomics](https://datacarpentry.org/organization-genomics/) | 

|            Miércoles 3 de Marzo              |
|---------------------------------|
|  Data cleaning with [OpenRefine](https://datacarpentry.org/OpenRefine-ecology-lesson/) |
| Parte 1 de [Git](https://swcarpentry.github.io/git-novice/)   |

|              Viernes 5 de Marzo              |
|---------------------------------|
|    Parte 2 de [Git](https://swcarpentry.github.io/git-novice/)  |


## Informacion General  
Aqui puedes encontrar un [documento colaborativo](https://docs.google.com/document/d/1M8Zy_DoDovuSDXQgjHfiwRrRUXyJQC3bPq_3VJYq9hQ/edit ) donde compartiremos información relevante, links, y respuestas a preguntas que surjan durante el taller. La mayor parte de las lecciones linux y git son parte del contenido habitual de [software carpentry](https://software-carpentry.org/) y [data Carpentry](https://datacarpentry.org/), organizaciones dedicada a enseñar habilidades de cómputo para hacer análisis de datos de forma reproducible, usaremos estas dos lecciones con su permiso. 
____________
# INSTALACIONES  
{% comment %}
Git Setup instructions rely on Shell instructions. If you don't include
Shell instructions as part of your workshop website, make sure to adjust
the text below accordingly.
{% endcomment %}
<div id="git">
  <h3>Git</h3>
  <p>
    Git is a version control system that lets you track who made changes
    to what when and has options for easily updating a shared or public
    version of your code
    on <a href="https://github.com/">github.com</a>. You will need a
    <a href="https://help.github.com/articles/supported-browsers/">supported
    web browser</a>.
  </p>
  <p>
    You will need an account at <a href="https://github.com/">github.com</a>
    for parts of the Git lesson. Basic GitHub accounts are free. We encourage
    you to create a GitHub account if you don't have one already.
    Please consider what personal information you'd like to reveal. For
    example, you may want to review these
    <a href="https://help.github.com/articles/keeping-your-email-address-private/">instructions
      for keeping your email address private</a> provided at GitHub.
  </p>

  <div>
    <ul class="nav nav-tabs" role="tablist">
      <li role="presentation" class="active"><a data-os="windows" href="#git-windows" aria-controls="Windows" role="tab" data-toggle="tab">Windows</a></li>
      <li role="presentation"><a data-os="macos" href="#git-macos" aria-controls="MacOS" role="tab" data-toggle="tab">MacOS</a></li>
      <li role="presentation"><a data-os="linux" href="#git-linux" aria-controls="Linux" role="tab" data-toggle="tab">Linux</a></li>
    </ul>

    <div class="tab-content">
      <article role="tabpanel" class="tab-pane active" id="git-windows">
        <p>
          Git should be installed on your computer as part of your Bash
          install (see the
          <a href="#shell">Shell installation instructions</a>).
        </p>
      </article>
      <article role="tabpanel" class="tab-pane" id="git-macos">
        <p>
          <strong>For macOS</strong>, install Git for Mac
          by downloading and running the most recent "mavericks" installer from
          <a href="http://sourceforge.net/projects/git-osx-installer/files/">this list</a>.
          Because this installer is not signed by the developer, you may have to
          right click (control click) on the .pkg file, click Open, and click
          Open on the pop up window.
          After installing Git, there will not be anything in your <code>/Applications</code> folder,
          as Git is a command line program.
          <strong>For older versions of OS X (10.5-10.8)</strong> use the
          most recent available installer labelled "snow-leopard"
          <a href="http://sourceforge.net/projects/git-osx-installer/files/">available here</a>.
        </p>
        <h4>Video Tutorial</h4>
        <div class="yt-wrapper2">
        <div class="yt-wrapper">
          <iframe type="text/html" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" src="https://www.youtube-nocookie.com/embed/9LQhwETCdwY?modestbranding=1&playsinline=1&iv_load_policy=3&rel=0" class="yt-frame" allowfullscreen></iframe>
        </div>
        </div>
      </article>
      <article role="tabpanel" class="tab-pane" id="git-linux">
        <p>
          If Git is not already available on your machine you can try to
          install it via your distro's package manager. For Debian/Ubuntu run
          <code>sudo apt-get install git</code> and for Fedora run
          <code>sudo dnf install git</code>.
        </p>
      </article>
    </div>
  </div>
</div>

# INSTALACIONES REQUERIDAS
<div id="openrefine">
  <h3>OpenRefine</h3>
  <p>
@@ -325,3 +226,78 @@ the text below accordingly.
    </div>
  </div>
</div>

{% comment %}
Git Setup instructions rely on Shell instructions. If you don't include
Shell instructions as part of your workshop website, make sure to adjust
the text below accordingly.
{% endcomment %}
<div id="git">
  <h3>Git</h3>
  <p>
    Git is a version control system that lets you track who made changes
    to what when and has options for easily updating a shared or public
    version of your code
    on <a href="https://github.com/">github.com</a>. You will need a
    <a href="https://help.github.com/articles/supported-browsers/">supported
    web browser</a>.
  </p>
  <p>
    You will need an account at <a href="https://github.com/">github.com</a>
    for parts of the Git lesson. Basic GitHub accounts are free. We encourage
    you to create a GitHub account if you don't have one already.
    Please consider what personal information you'd like to reveal. For
    example, you may want to review these
    <a href="https://help.github.com/articles/keeping-your-email-address-private/">instructions
      for keeping your email address private</a> provided at GitHub.
  </p>

  <div>
    <ul class="nav nav-tabs" role="tablist">
      <li role="presentation" class="active"><a data-os="windows" href="#git-windows" aria-controls="Windows" role="tab" data-toggle="tab">Windows</a></li>
    <ul class="nav nav-tabs" role="tablist">	    
      <li role="presentation"><a data-os="macos" href="#git-macos" aria-controls="MacOS" role="tab" data-toggle="tab">MacOS</a></li>
      <li role="presentation"><a data-os="linux" href="#git-linux" aria-controls="Linux" role="tab" data-toggle="tab">Linux</a></li>
    </ul>

    <div class="tab-content">
      <article role="tabpanel" class="tab-pane active" id="git-windows">
        <p>
          Git should be installed on your computer as part of your Bash
          install (see the
          <a href="#shell">Shell installation instructions</a>).
        </p>
      </article>
      <article role="tabpanel" class="tab-pane" id="git-macos">
        <p>
          <strong>For macOS</strong>, install Git for Mac
          by downloading and running the most recent "mavericks" installer from
          <a href="http://sourceforge.net/projects/git-osx-installer/files/">this list</a>.
          Because this installer is not signed by the developer, you may have to
          right click (control click) on the .pkg file, click Open, and click
          Open on the pop up window.
          After installing Git, there will not be anything in your <code>/Applications</code> folder,
          as Git is a command line program.
          <strong>For older versions of OS X (10.5-10.8)</strong> use the
          most recent available installer labelled "snow-leopard"
          <a href="http://sourceforge.net/projects/git-osx-installer/files/">available here</a>.
        </p>
        <h4>Video Tutorial</h4>
        <div class="yt-wrapper2">
        <div class="yt-wrapper">
          <iframe type="text/html" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" src="https://www.youtube-nocookie.com/embed/9LQhwETCdwY?modestbranding=1&playsinline=1&iv_load_policy=3&rel=0" class="yt-frame" allowfullscreen></iframe>
        </div>
        </div>
      </article>
      <article role="tabpanel" class="tab-pane" id="git-linux">
        <p>
          If Git is not already available on your machine you can try to
          install it via your distro's package manager. For Debian/Ubuntu run
          <code>sudo apt-get install git</code> and for Fedora run
          <code>sudo dnf install git</code>.
        </p>
      </article>
    </div>
  </div>
</div>
