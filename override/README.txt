és un exemple del override

bascament consisteix en 
1/ 
afegit
<meta http-equiv="content-type" content="text/html; charset=utf-8"/>
al principi de tot pq funcioni el format dels strings

2/ script al final

</script>
<script language="JavaScript" type="text/JavaScript">
// font
// https://www.youtube.com/watch?v=PT6xsr_AUQ0
// https://www.youtube.com/watch?v=0Zh909IfutE
// https://www.youtube.com/watch?v=_pxRodW4zbs
// console.log('fff');

// important
// he hagut d'afegir 
// <meta http-equiv="content-type" content="text/html; charset=utf-8"/>
// al head per que els txt s'interpretin ok

// anar eliminant primer item cada com que faig un enviament
let items = [
// {para: 'marcaltl;', asunto:'prova1', txtBody: 'prova1\naaa'},
 {para: 'marcaltl', asunto: 'Licencia Meteonorm', txtBody: 'Hola Fernando Acuña Andrea,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: SUBC-AXRO-JRME-WOGU<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'fernandoaa1;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Fernando Acuña Andrea,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: SUBC-AXRO-JRME-WOGU<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'roxanabh1;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Roxana Barbes Hernández,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: SUHD-MWGF-VMYH-UIYH<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'karlab;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Karla Briceño,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: PVJW-PFJF-DTCD-VMKJ<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'stefaniab1;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Stefania Buzatu,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: YLFU-MLCS-CRIJ-TOWZ<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'joseet3;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola José Andrés Espinoza Tillería,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: RTQT-PLCO-TFCD-WESG<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'raulgn1;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Raúl García Núñez,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: HSOC-RDXE-EZFR-LPTZ<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'gustavojo;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Gustavo Jiménez Obando,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: SGDX-JJJA-EGVI-PACE<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'lydialc;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Lydia López Criado,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: TCIV-JBXP-LDAF-JTNR<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'lizethlr;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Lizeth Viridiana López Rincón,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: VIQN-JGNE-DGUV-ZXZZ<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'claudiams1;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Claudia Márquez Sala,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: WZJL-VIIJ-WYRB-RSID<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'agustinap4;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Agustina Sol Peiretti,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: QNHN-GGGB-ZLRS-OSKG<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'soniarc2;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Sonia Carolina Ramirez Cavero,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: PXLJ-PZGZ-PTFP-TVTS<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'victoriare1;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Victoria Rios Esteve,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: DSAG-OHCG-EGBP-XNPL<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'estebanrr1;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Esteban Emiliano Romero Romero,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: YMNB-NCHT-STGZ-IOUA<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'cintiasj;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Cintia Saavedra Jaldin,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: ELTJ-ORJB-DHYL-GACW<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
// {para: 'mariav13;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola María Florencia Verzellini,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: ALJK-OOSL-TJKD-KVAD<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},
//{para: 'samirayh;marcaltl;carlesga1', asunto: 'Licencia Meteonorm', txtBody: 'Hola Samira Antonia Yávar Herrera,<br><br>A continuación encuentra el código con el que deberás activar tu software Meteonorm:<br><br>CODIGO: FHZI-JTGS-MNGM-ZLNQ<br><br>Recuerda que, en caso que en un futuro quieras desinstalar Meteonorm, debes “desactivar” la licencia antes de iniciar el proceso de desinstalar. De lo contrario no podrás seguir usando el tu código de activación en otro Meteonorm que vayas a instalar.<br><br>Carles y Marçal'},

];



let per = document.getElementsByName('para_logins')[0];
let assumpte = document.getElementById('titolmissatge');
let btxtBody = document.getElementsByName('textmissatge_html')[0] 

per.value = items[0].para;
assumpte.value = items[0].asunto;
var newww =  items[0].txtBody;
btxtBody.innerHTML =  newww;
</script>