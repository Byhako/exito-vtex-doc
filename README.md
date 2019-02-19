---


---

<h1 id="éxito-vtex-io">Éxito (Vtex IO)</h1>
<p>Esta documentación es una guía para el desarrollo con <strong>Vtex IO</strong></p>
<ul>
<li><a href="#recursos- necesarios">Recursos-necesarios</a></li>
<li><a href="#gu%C3%ADa">Guía</a></li>
<li><a href="#vtex-cli">Vtex Cli</a></li>
<li><a href="#trabajandocon-Vtex-eact](#trabajandocon vtex </li>
<li><a href="#l-y-react)
* [Lista-decomponentes-actuales">Lista-d -componentes</a></li>
<li><a href="#integraci%C3%B3n-continuantegración -continua</a></li>
</ul>
<h2 id="recursos-necesarios">Recursosnecesarios</h2>
<ol>
<li><a href="https://nodejs.org/es/">Node js</a></li>
<li>< https://yarnpkg.com/en/">Yarn</a> Gestor de paquetes de Facebook</li>
<li><a href="(https://code.visualstudio.com/">Visual Studio Code</a>) Editor<br>
	2.1 Extensiones Básicas:
<ul>
<li><a href="https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets">ES7 React/Redux/GraphQL/React-Native snippets</a></li>
<li><a href="https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify">Beautify</a></li>
<li><a href="https://marketplace.visualstudio.com/items?itemName=steoates.autoimport">Auto Import</a></li>
<li><a href="https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint">EsLint</a></li>
<li><a href="https://marketplace.visualstudio.com/items?itemName=pflannery.vscode-versionlens">Version Lens</a></li>
</ul>
</li>
<li><a href="epohttps://github.com/facebook/create-react-app">Create React App Repo</a></li>
<li><a href="https://www.npmjs.com/package/create-react-app">Create React App Npm</a></li>
<li><a href="https://www.npmjs.com/package/vtex">Vtex Cli</a>) Linea de comandos para vtex</li>
<li><a href="https://www.npmjs.com/package/exito-cli">Exito Cl Linea de comandos para éxito</li>
<li><a href="http://cmder.net/">CMDER</a>) Terminal Para windows</li>
<li><a href="https://www.iterm2.com/">Iterm2</ Terminal para Mac</li>
<li><a href="https://docs.aws.amazon.com/cli/latest/userguide/install-windows.html">Aws Cli</a>) Linea de comandos para Amazon</li>
</ol>
<h2 id="guía">Guía</h2>
<h3 id="cursos-para-iniciar">Cursos para iniciar</h3>
<p>React Básico <a href="https://www.youtube.com/watch?v=bG53Pw17tog&amp;list=PLeWI3XlFEVOX6jACDygzApsvigQiDrun8">Youtube CodeJobs</a><br>
React Curso Completo <a href="https://exito.udemy.com/react-the-complete-guide-incl-redux/learn/v4/overview">Udemy</a><br>
Graphql + React <a href="[Udehttps://exito.udemy.com/graphql-with-react-course/learn/v4/content">Udemy</a><br>
Guía <a href="http://aprendegit.com/que-es-git-flow/">Gitflow</a><br>
<a href="](https://github.com/sw-yx/react-typescript-cheatsheet">React typescript tips</a></p>
<h3 id="como-manejar-la-versión-de-los-componentes-semantic-versioning">Como manejar la versión de los componentes (Semantic versioning)</h3>
<p>

para manejar la versión de nuestros componentes emplearemos la siguiente guía <a href="https://docs.npmjs.com/about-semantic-versioning">semantic-versioning</a></p>
<h3 id="como-se-deben-de-documentar-el-código-en-react">Como se deben de documentar el código en React</h3>
<p>

Para realizar la documentación en React se empleara el estándar definido por <a href="https://react-styleguidist.js.org/docs/documenting.html">react-styleguidist</a> donde se definen diversas técnicas necesarias para documentar los componentes creados, ademas de esto permite generar una documentación automática que permite visualizar muy bien el contenido que hemos documentado. <a href="https://github.com/styleguidist/react-styleguidist/tree/master/examples/basic">demo</a></p>
<p>Se recomienda manejar el concepto de <a href="http://usejsdoc.org/">jsDoc</a> para los comentarios de nuestros componentes.</p>
<p>

Para la documentemlearemos los archivos</p>
<ul>
<li><a href="http://Changelog.md">Changelog.md</a></li>
<li><a href="http://Readme.md">Readme.md</a></li>
</ul>
<h3 id="ejemplos-para-documentar">Ejemplos para documentar:</h3>
<p><a href="httpecommerce/exito-vtex-doc/blob/master/resources/examples/components/documentationMaik3345/exito-vtex-doc/tree/master/CHANGELOG-BASIC.md">)
[Basic Changelog</a><br>
<a href="Readme](https://github.com/grupo-exito-ecommerceMaik3345/exito-vtex-doc/blob/master/resources/examples/components/documentation/README-BASIC.mdBasic/a></p>
<h3 id="definición-para-los-workspace-empleados-en-el-desarrollo">Definición para los workspace empleados en el desarrollo</h3>
<p>

Se plantea la siguiente estructura, donde <strong>exito</strong> es el workspace principal o productivo, el workspace <strong>develop</strong> es el workspace pre productivo y los workspaces <strong>**qa1, qa2, qa3</strong>** son los workspace destinados para los equipos de SQA para realizar las validaciones de los desarrollos que se planteen para el sprint. Cada desarrollador deberá de crear su workspace definiendo el equipo de SQA que realizara sus validaciones técnicas y el tipo de desarrollo que esta realizando en ese momento.</p>
<h4 id="ejemplo">Ejemplo:</h4>
<ul>
<li><strong>qa1_header–exito.myvtex.com</strong></li>
</ul>
<p><strong>qa1</strong>  —&gt; Equipo de SQA encargado de la validación técnica<br>
<strong>header</strong> —&gt; Desarrollo asignado</p>
<h4 id="jerarquia-de-los-workspace">Jerarquia de los workspace</h4>

<table>
<thead>
<tr>
<th></th>
<th><a href="exito.myvtex">exito</a></th>
<th></th>
</tr>
</thead>
<tbody>
<tr>
<td></td>
<td><strong><a href="https://develop--exito.myvtex.com/">develop</a></strong></td>
<td></td>
</tr>
<tr>
<td><strong><a href="https://qa1--exito.myvtex.com/">qa1</a></strong></td>
<td><strong><a href="https://qa2--exito.myvtex.com/">qa2</a></strong></td>
<td><strong><a href="https://qa3--exito.myvtex.com/">qa3</a></strong></td>
</tr>
<tr>
<td>qa1_sprint</td>
<td>qa2_sprint</td>
<td>qa3_sprint</td>
</tr>
</tbody>
</table><h2 id="vtex-cli">Vtex Cli</h2>
<ul>
<li><a href="#creaci%C3%B3n-nuevo- componentevtex-cli">C](#creación -de -un -nuevo -componente</a></li>
<li><a href="#instalaci%C3%B3n-ación de- dependencias- para- el-a Admin- de-v Vtex">I](#instalación dedependencias -para -el A-admin de Vtex</a></li>
<li><a href="#creaci%C3%B3n-de-un-nuevo-componente-con-exito-cli">-de-vtex)
*  [Creación de un deunnuevocomponente con Exito cli</a></li>
</ul>
<h3 id="reacióndeunnuevocomponente-con-vtex-cli">Creación de un nuevo componente con Vtex cli</h3>
<p>

para la creación de un nuevo proyecto empleamos el comando <code>vtex init</code>` el cual nos da las siguientes opciones<br>
<code>vtex init</code></p>
<pre class=" language-bash"><code class="prism  language-bash"> react getting-started
 graphql getting-started
 react+graphql
 hello graphql
 hello react
 dreamstore getting-started
</code></pre>
<h3 id="creación-de-un-nuevo-componente-con-exito-cli">Creación de un nuevo componente con Exito cli</h3>
<p><code>exito init</code></p>
<pre class=" language-bash"><code class="prism  language-bash"> hello-react-typescript
</code></pre>
<h3 id="repositorio--  de- los- proyectos">Repositoriodelosproyectos</h3>
<p><a href="https://github.com/grupo-exito-ecommerceMaik3345/hello-react-ts">hello-react-typescript github</a></p>
<h3 id="instalación-de-dependenciasparaeldminInstalación de dependencias para el Admin de Vtex</h3>
<p>

Las siguientes dependencias permiten agregar comportamientos como el admin pages y el storefront en la página de vtex.</p>
<pre><code>vtex install vtex.pages-editor
vtex install vtex.admin-pages
</code></pre>
<h2 id="trabajando-con-vtex-y-react">Trabajando con Vtex y React</h2>
<ul>
<li><a href="%C3%B3ón-de-un-componente-editable-en-el-storefront-de-vtex">Configuración para el StoreFront</a></li>
<li><a href="#p)
* [Promoverworkspace-a-s a producci%C3%B3n">Pón](#promover -un-workspaces a -a-producción</a></li>
</ul>
<hr>
<h3 id="configuración-de-un-componente-editable-en-el-storefront-de-vtex">Configuración de un componente editable en el StoreFront de Vtex</h3>
<p>

para la configuración necesaria para el storefront se necesitan tres métodos dentro de nuestro componente:</p>
<ol>
<li><em>


1. *getSchema</em>* : Define los diferentes atributos que se le pasarán al componente por medio de las propiedades.</li>
</ol>
<pre class=" language-bash"><code class="prism  language-bash">ClassName.getSchema  <span class="token operator">=</span>  <span class="token punctuation">(</span><span class="token punctuation">)</span>  <span class="token operator">=</span><span class="token operator">&gt;</span>  <span class="token punctuation">{</span>
	<span class="token keyword">return</span>  <span class="token punctuation">{</span><span class="token punctuation">}</span>
<span class="token punctuation">}</span><span class="token punctuation">;</span>
</code></pre>
<p>
```bash
ClassName.getSchema  =  ()  =>  {
	return  {}
};
```
Ejemplos donde se emplean esquemas en los componentes:</p>
<ul>
<li><a href="
* [Vtex Carousel](https://github.com/vtex-apps/carousel">Vtex Carousel</a></li>
<li><a href="https://github.com/vtex-apps/minicart">Vtex Minicart</a></li>
</ul>
<ol start="2">
<li><em>)
* [Vtex Minicart](https://github.com/vtex-apps/minicart)

2. *propTypes</em>* : Permite tipar los datos y definir de que tipo son cada uno de los atributos pasados por las props del componente</li>
</ol>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">import</span>  PropTypes  from  <span class="token string">
```bash
import  PropTypes  from  'prop-types'</span>

ClassName.propTypes  <span class="token operator">=</span> <span class="token punctuation">{</span><span class="token punctuation">}</span><span class="token punctuation">;</span>
</code></pre>
<ol start="3">
<li><em>= {};
```
 3. *defaultProps</em>* : Permite definir cual va a ser el valor por defecto para nuestros atributos pasados por los props del componente.</li>
</ol>
<pre class=" language-bash"><code class="prism  language-
```bash">
ClassName.defaultProps  <span class="token operator">=</span> <span class="token punctuation">{</span><span class="token punctuation">}</span><span class="token punctuation">;</span>
</code></pre>
<p>= {};


Estos tres métodos son empleados por Vtex para la creación de las opciones del storeFront</p>
<p>Ejemplo <a href="

Ejemplo [aquí](https://github.com/grupo-exito-ecommerceMaik3345/exito-vtex-doc/blob/master/resources/examples/components/schema-examples/basic-shecma-js.js">aquí</a></p>
<h2 id="promover-un-workspaceproducción">)



## Promover un workspace a producción</h2>
<p>


los pasos para promover un workspace son:</p>
<ol>
<li><code>
1. `vtex workspace production true</code>`  Cambiamos el modo producción del workspace a true</li>
</ol>
<h4 id="callback">callback</h4>
<pre class=" language-bash"><code class="prism  language-bash">info:    Workspace dev <span class="token keyword">set</span>
#### callback 
````bash
info:    Workspace dev set to production mode
info:    You can now check your changes before publishing them
info:    If everything is fine, promote with vtex promote
</code></pre>
<ol start="2">
<li><code>````
2. `vtex publish [path]</code>` Publicar todos los componentes o los componentes que vallamos a emplear, para realizar la publicación de un componente debemos de tener en cuenta el orden de importancia de los componentes. de lo contrario obtendremos error al subir los componentes</li>
<li><code>
3. `vtex promote</code>` Promovemos el workspace actual a ser una integración con el master, este paso eliminara el workspace actual.</li>
</ol>
<h2 id="como-publicar-una-aplicación">

## Como publicar una aplicación</h2>
<ol>
<li><code>

1. `vtex workspace production true</code>`  Cambiamos el modo producción del workspace a true</li>
<li><code>
2. `vtex publish [path]</code>` Publicar todos los componentes o los componentes que vallamos a emplear, para realizar la publicación de un componente debemos de tener en cuenta el orden de importancia de los componentes. de lo contrario obtendremos error al subir los componentes, ademas se debe de tener en cuenta la versión de la aplicación.</li>
<li>
3. Luego de publicar los componentes, volvemos a indicar que el workspace esta en modo desarrollo <code>`vtex workspace production false</code></li>
</ol>
<h2 id="lista-de-componentes-actuales-en-react">`

## Lista de componentes actuales en React</h2>
<pre><code>

```
|- exito.vtex-components
|- exito.login
|- exito.product-carousel
|- exito.minicart
|- exito.carousel
|- exito.category-menu
|- exito.components
|- exito.footer
|- exito.header
|- exito.home-configuration
|- exito.geolocation
|- exito.cart-detail
|- exito.login
|- exito.producto
|- exito.product-details
|- exito.product-images-list
|- exito.product-summary
|- exito.search-result
|- exito.shelf
|- exito.store
|- exito.vtex-components
| +- ...
</code></pre>
<h2 id="lista-de-componentes-actuales-en-node--graphql">```

## Lista de componentes actuales en Node + Graphql</h2>
<pre><code>

```
|- exito.bags
|- exito.smartquick
| +- ...
</code></pre>
<h2 id="integración-continua">```



## Integración continua</h2>
<p>
Los recurso necesarios para el proceso de integración continua son los siguientes</p>
<pre><code>
```
|-config
|--docker
|---develop.dockerfile
|---master.dockerfile
|--aws
|---develop-buildspec.yml
|---master-buildspec.yml
|--sonar
|---sonar-project.properties
| +- ...
</code></pre>
<p>```

Pueden encontrar la especificación técnica de los archivo en el documento en <a href="[Github](https://github.com/grupo-exito-ecommerce/exito-vtex-doc/blob/master/directory/continuos-integration-config/continuos-integration-config.mdCONTINUOS-INTEGRATION-SPECIFICATION.md%22%3EGithub">Github</a></p>
<h4 id="c">Github)

#### Configuración- de- los- recursos- con- [exito-cli">Configuración de los recursos con <a href="https://www.npmjs.com/package/exito">exito-cli</a></h4>
<h4 id="comandos-a-emplear">Comandos a emplear:</h4>
<ol>
<li><code>](https://www.npmjs.com/package/exito)


#### Comandos a emplear:
1. `exito generate config</code>`:  Comando que genera las carpetas necesarias de configuración para <a href="[Cloud-Formation](https://docs.aws.amazon.com/cloudformation/index.html">Cloud-Formation</a>  y <a href="https://www.sonarqube.org/">SonarQube</a></li>
<li><code>)  y [SonarQube](https://www.sonarqube.org/)
2.  `exito generate template [name-repository]</code>:</li>
</ol>
<p>`: 
		
Comando que genera los archivo  <code>`develop-template.json</code> y <code>` y `master-template.json</code>` estos archivos son empleados para montar la infraestructura con <a href="[Cloud-Formation](https://docs.aws.amazon.com/cloudformation/index.html">Cloud-Formation</a>), para ver la guía de como subir los templates a Cloud-Formation ver la siguiente documentación <a href="[Cloud-Formation-Doc](https://github.com/grupo-exito-ecommerce/exito-vtex-doc/blob/master/directory/cloud-formation/cloud-formation-documentation.md">Cloud-Formation-Doc</a>).</p>
<h1 id="proceso-de-migración-vtex-v2">)).



# Proceso de migración Vtex v2</h1>
<p>

Actualización en el archivo manifest.json</p>
<pre><code>

```
"vtex-version": "0.0.0",  
"builders": {  
	"react": "3.x",  
	"styles": "1.x",  
	"store": "0.x",  
	"messages": "0.x"  
},
</code></pre>
<h4 id="guía-1">Guía:</h4>
<p><code>```
#### Guía:
`vtex-version</code>`:  Atributo empleado con la finalizad de mantener registrada la ultima versión del componente de vtex, la idea con este atributo es ir actualizando gradualmente cuando vtex lance versiones de los componentes que estemos personalizando y mantener el registro que indique cual fue la ultima versión de vtex empleada, si el componente no es creado por vtex aun así agregamos el atributo dejando en la versión <code>0.0.0</code>`0.0.0` para así mantener la misma estructura en todos los proyectos.</p>
<p><code>

`
"styles": "1.x",  
"store": "0.x",</code>  
`: Nueva configuración para compilar la aplicación de vtex, se ha removido el builder <code>`"pages": "0.x"</code>`, Pueden encontrar una guía detallada de la migración de estos builders en <a href="[vtex help](https://help.vtex.com/es/tutorial/conociendo-el-storebuilder-y-el-stylesbuilder">vtex help</a></p>
<p><code>)

`"messages": "0.x"</code>  `: Nueva configuración para la traducción de nuestro componente.</p>
<h4 id="eliminación-de-la-carpeta-pages-y-creación-del-directorio-store">


#### Eliminación de la carpeta pages y creación del directorio store</h4>
<p>

Con los cambios en el builder, vtex reemplazo la lógica para armar las url y los contenedores de nuestra aplicación, pueden encontrar la explicación técnica armada por vtex <a href="[vtex help](https://help.vtex.com/es/tutorial/conociendo-el-storebuilder-y-el-stylesbuilder">vtex help</a></p>
<pre><code>)

```
|-pages ✗
|--pages.json ✗
|-store ✓
|--blocks.json ✓
|--interface.json ✓
|--routes.json ✓
| +- ...
</code></pre>```

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE1MTgyMTczNl19
-->