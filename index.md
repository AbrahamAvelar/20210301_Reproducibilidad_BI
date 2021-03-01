  
    
          Introducción a reproducibilidad en bioinformática

# Bioinformática  
![langebio](images/langebio.png)  

En este curso aprenderás un poco de las herramientas linux, git, OpenRefine. También revisaremos buenas prácticas en organización de archivos y tablas con datos para biología.  



## Calendario  

|        Lunes 1 de Marzo             |            Miércoles 3 de Marzo                 |      Viernes 5 de Marzo              |
----------------------------------|--------------------------------------|-------------------------------------------------|
Septiembre 20 [Linux bash](https://swcarpentry.github.io/shell-novice-es/)               |   Parte 1 de [Git](https://swcarpentry.github.io/git-novice/)   |    Parte 2 de [Git](https://swcarpentry.github.io/git-novice/)  |

## Informacion General  
Aqui puedes encontrar un [documento colaborativo](https://etherpad.net/p/bioinformatica  ) donde compartiremos información relevante, links, y respuestas a preguntas que surjan durante el taller. Dos de nuestras lecciones linux y git son parte del contenido habitual de [software carpentry](https://software-carpentry.org/) una organización dedicada a enseñar habilidades de cómuto para hacer más en menos tiempo y con menos sufrimiento, usaremos estas dos lecciones con su permiso. Las otras dos lecciones fueron pensadas de acuerdo a las necesidades específicas de nuestro centro de trabajo.   

## Temario detallado  
<table> <tr><td> <b> Tema 1 Linux bash </b> <br>
1.1 Linux/Unix, Principios básicos del Shell  <br>
1.2 Comandos para el manejo de archivos y directorios   <br>
1.3 Loops   <br>
1.4 Manejo de Scripts    <br>
1.5 Encontrar información: grep y find. <br> </td>
    <td> <b> Tema 2  Google y la organización de documentos </b><br>
2.1 Formas: Crear encuestas presentables. <br>
2.2 Drive documentos del laboratorio, compartir documentos <br>
2.3 Sites crear una página para el laboratorio <br>
2.4 Calendar Organizar la agenda. <br>
2.5 Tareas Organizar las tareas diarias. <br></td></tr>
    <tr><td> <b> Tema 3  El respaldo y documentación de scripts </b> <br>
3.1 La importancia de documentar y respaldar el trabajo informático <br>
3.2 Git Guardar los scripts en internet <br>
3.3 MD Crear documentación organizada <br>
3.4 Wiki git Documentar extensivamente scripts <br>
3.5 Ejemplos: R también tiene markdown (MD) para documentar procedimientos <br>
Docker y la repetibilidad de resultados en maquinas <br></td>
      <td> <b> Tema 4  Herramientas de genómica </b> <br>  
4.1 Descargar datos NCBI (Linux) <br>  
4.2 Cómo tomar metadatos en proyectos genómicos <br>  
4.3 MicroReact y la visualización de metadatos. <br>  
4.4 Editar archivos para microreact: One liners <br>  
4.5 Seaview crear un arbol para microreact. <br>   </td> </tr> </table>    
       
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

<div id="openrefine">
  <h3>OpenRefine</h3>
  <p>
    For this lesson you will need <em>OpenRefine</em> and a
    web browser. <em>Note:</em> this is a Java program that runs on your machine (not in the cloud).
    It runs inside a web browser, but no web connection is needed.
  </p>

  <div>
    <ul class="nav nav-tabs" role="tablist">
      <li role="presentation" class="active"><a data-os="windows" href="#openrefine-windows" aria-controls="Windows" role="tab" data-toggle="tab">Windows</a></li>
      <li role="presentation"><a data-os="macos" href="#openrefine-macos" aria-controls="MacOS" role="tab" data-toggle="tab">MacOS</a></li>
      <li role="presentation"><a data-os="linux" href="#openrefine-linux" aria-controls="Linux" role="tab" data-toggle="tab">Linux</a></li>
    </ul>

    <div class="tab-content">
      <article role="tabpanel" class="tab-pane active" id="openrefine-windows">
        <ol>
          <li>
            Check that you have either the Firefox or the Chrome browser installed and set as your default browser.
            <strong>OpenRefine runs in your default browser.</strong>
            It will not run correctly in Internet Explorer.
          </li>
          <li>Download software from <a href="http://openrefine.org/">http://openrefine.org/</a></li>
          <li>Create a new directory called OpenRefine.</li>
          <li>Unzip the downloaded file into the OpenRefine directory by right-clicking and selecting "Extract ...". </li>
          <li>Go to your newly created OpenRefine directory.</li>
          <li>Launch OpenRefine by clicking <code>openrefine.exe</code> (this will launch a command prompt window, but you can ignore that - just wait for OpenRefine to open in the browser).</li>
          <li>If you are using a different browser, or if OpenRefine does not automatically open for you, point your browser at <a href="http://127.0.0.1:3333/">http://127.0.0.1:3333/</a> or <a href="http://localhost:3333">http://localhost:3333</a> to use the program.</li>
        </ol>
      </article>
      <article role="tabpanel" class="tab-pane" id="openrefine-macos">
        <ol>
          <li>Check that you have either the Firefox or the Chrome browser installed and set as your default browser. <strong>OpenRefine runs in your default browser.</strong> It may not run correctly in Safari.</li>
          <li>Download software from <a href="http://openrefine.org/">http://openrefine.org/</a>.</li>
          <li>Create a new directory called OpenRefine.</li>
          <li>Unzip the downloaded file into the OpenRefine directory by double-clicking it.</li>
          <li>Go to your newly created OpenRefine directory.</li>
          <li>Launch OpenRefine by dragging the icon into the Applications folder.</li>
          <li>Use <kbd>Ctrl</kbd>-click/Open ... to launch it.</li>
          <li>If you are using a different browser, or if OpenRefine does not automatically open for you, point your browser at <a href="http://127.0.0.1:3333/">http://127.0.0.1:3333/</a> or <a href="http://localhost:3333">http://localhost:3333</a> to use the program.</li>
        </ol>
      </article>
      <article role="tabpanel" class="tab-pane" id="openrefine-linux">
        <ol>
          <li>Check that you have either the Firefox or the Chrome browser installed and set as your default browser. <strong>OpenRefine runs in your default browser.</strong></li>
          <li>Download software from <a href="http://openrefine.org/">http://openrefine.org/</a>.</li>
          <li>Make a directory called OpenRefine.</li>
          <li>Unzip the downloaded file into the OpenRefine directory.</li>
          <li>Go to your newly created OpenRefine directory.</li>
          <li>Launch OpenRefine by entering <code>./refine</code> into the terminal within the OpenRefine directory.</li>
          <li>If you are using a different browser, or if OpenRefine does not automatically open for you, point your browser at <a href="http://127.0.0.1:3333/">http://127.0.0.1:3333/</a> or <a href="http://localhost:3333">http://localhost:3333</a> to use the program.</li>
        </ol>
      </article>
    </div>
  </div>
</div>



