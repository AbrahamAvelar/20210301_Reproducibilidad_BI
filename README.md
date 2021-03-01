# Reproducibilidad_BI
Clase de reproducibilidad en bioinformática

# Bioinformática  
![langebio](imagenes/langebio.png)  

En este curso aprenderás un poco de las herramientas linux, git, Google docs y microreact.  



## Calendario  

|        Lunes 1 de Marzo             |            Miércoles 3 de Marzo                 |      Viernes 5 de Marzo              |
----------------------------------|--------------------------------------|-------------------------------------------------|
Septiembre 20 [Linux bash](https://swcarpentry.github.io/shell-novice-es/)               |   Septiembre 27 [Git](paginas/git/sesion3.md) y [markdown](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)       |    Octubre 4  Proyectos y/o temas específicos.  |
Septiembre 21 [Google drive](paginas/drive/sitios.md)        |  Septiembre 28 [Metadatos y visualización](paginas/genomica/genomica.md)|    Octubre 5  Presentación de proyecto.         | 

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
## Instalaciones y requerimientos previos  
<h2 id="setup">Setup</h2>  

<p>
  Para participar en este taller necesitas acceso al siguiente software. Además necesitarás acceso a un navegador como chrome o firefox.   
  </p>
<p>
  Aqui hay una referencia de posibles problemas durante la instalación.  
  <a href = "{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Wiki de problemas de instalación y sus soluciones. </a>.
</p>

<div id="shell">  
  <h3>El Bash Shell</h3>  
  <p>  
    Bash es un intérprete de comandosque te da poder de hacer tareas simples rápidamente.  
  </p>  

  <div class="row">  
    <div class="col-md-4">  
      <h4 id="shell-windows">Windows</h4>  
      <a href="https://www.youtube.com/watch?v=339AEqk9c-8">Video Tutorial</a>  
      <ol>  
        <li>Baja para windows <a href="https://git-for-windows.github.io/">el instalador de git </a>.</li>  
        <li>Corre el instalador y sigue los siguientes pasos:  
          <ol>  
            <li>Click en "Next".</li>  
            <li>Click en "Next".</li>    
            <li>  
              <strong>  
               Manten el "Use Git from the Windows Command Prompt" seleccioinado y  click en "Next".  
              </strong>  
                Si se te olvida hacer esto algunos programas que necesitarás no funcionaran correctamente.  
                Si esto te pasa regrésate al paso anterior del instalador y selecciona la opción correcta.  
            </li>  
            <li>Click en "Next".</li>
            <li>  
              <strong>  
                Mantén "Checkout Windows-style, commit Unix-style line endings" seleccionado y click en "Next".
              </strong>
            </li>
            <li>  
              <strong>  
                Mantén "Use Windows' default console window" seleccionado y click en "Next".  
              </strong>  
            </li>  
            <li>Click en "Install".</li>
            <li>Click en "Finish".</li>  
          </ol>  
        </li>  
        <li>  
          si tu variable de ambiente "HOME" no está lista (o no sabes qué es esto):
          <ol>
            <li>Abre el prompt (Abre el menu start, escribe <code>cmd</code> y presiona enter [Enter])</li>
            <li>
              Escribe la siguiente línea en la ventana del promt exactamente como se  muestra:  
              <p><code>setx HOME "%USERPROFILE%"</code></p>  
            </li>  
            <li>Presiona [Enter], debes de ver <code>SUCCESS: Specified value was saved.</code></li>
            <li>Para salir del prompr escribe <code>exit</code> y presiona enter [Enter]</li>
          </ol>
        </li>
      </ol>
      <p>Esto te dará ambos Git y Bash en el programa Git Bash.</p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-macosx">macOS</h4>
      <p>
        El shell por default en todas las versiones de macOS es Bash, asi que no debes instalar nada.  Podrás accesar a Bash desde la Terminal
        (que se encuentra en        <code>/Applications/Utilities</code>).
        Para la instalación de Git aqui tenemos un <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">video tutorial</a>
        for an example on how to open the Terminal.
        Tal vez quieras mantener la Terminal en tu dock para este taller.  
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-linux">Linux</h4>
      <p>
        El shell es usualmente Bash, pero si tu máquina es diferente puedes abrir una terminal y escribir <code>bash</code>.  
        No se necesita intalar nada
      </p>
    </div>
  </div>
</div> 

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



