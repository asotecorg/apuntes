# Instalado Apache Tomcat https://vistatotal.com/anexoCRS-1.0/
_ 
_ 
- 
-
#Cambios a realizar cuando hay nueva instalación
- Crear usuario para la empresa.
 en la carpeta WEB-INF/template/coops/ crear nueva carpeta para la empresa y realizar los siguietentes cambios
## formulario.html 
- - th:action="@{/coops/coopcica/search}" --> poner carpeta de la carpeta.
- - input type="hidden" name="empresa" value="23"/  --> poner el cod_empresa  en el value                                                          
- - input type="hidden" name="nomempresa" value="coacairo"/>  --> poner el carpeta de la empresa
## formulario-no-residentes.html 
- -  form class="user"   action="#" th:action="@{${uri}?  ${uri} : '/coops/coopcica/edit'}" --> poner el nombre de la empresa
- - input type="hidden" name="nomempresa" value="coopcica"/> --> poner el carpeta de la empresa

## formulario-residentes.html 
- -  form class="user"   action="#" th:action="@{${uri}?  ${uri} : '/coops/coopcica/edit'}" --> poner el nombre de la empresa
- - input type="hidden" name="nomempresa" value="coopcica"/> --> poner el carpeta de la empresa

## reporte.html 
- -  form class="user"   action="#" th:action="@{${uri}?  ${uri} : '/coops/coopcica/edit'}" --> poner el nombre de la empresa
- - input type="hidden" name="nomempresa" value="coopcica"/> --> poner el carpeta de la empresa
