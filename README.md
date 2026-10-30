# State of Mexico: law history in git

The law of the State of Mexico (Estado Libre y Soberano de México, Mexico) as a git history: one file per article, one commit per publication that changed it, dated the day it took effect, with the decree as the commit's author. `git blame` names the decree behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `mx-mex/`. Mexico's federal law is in [lexifina/mexico-law](https://github.com/lexifina/mexico-law).

The text is in Spanish, exactly as the source prints it.

## What this repository holds

133 ordenamientos with 1643 versions so far: the constitution first, then the codes and laws in force, added in parts. Regulations, decrees and repealed laws are not included yet.

| Folder | Ordenamiento | Versions | History |
| --- | --- | ---: | --- |
| `constitucion-politica/` | CONSTITUCION POLITICA DEL ESTADO LIBRE Y SOBERANO DE MEXICO | 235 | as first published, then each reform: 13 November 1917 to 26 September 2026 |
| `codigo-administrativo/` | CODIGO ADMINISTRATIVO DEL ESTADO DE MEXICO | 217 | as first published, then each reform: 13 March 2002 to 26 September 2026 |
| `codigo-civil/` | CODIGO CIVIL DEL ESTADO DE MEXICO | 83 | as first published, then each reform: 22 June 2002 to 17 June 2026 |
| `codigo-de-procedimientos-administrativos/` | CODIGO DE PROCEDIMIENTOS ADMINISTRATIVOS DEL ESTADO DE MEXICO | 38 | as first published, then each reform: 9 March 1997 to 25 September 2026 |
| `codigo-de-procedimientos-civiles/` | CODIGO DE PROCEDIMIENTOS CIVILES DEL ESTADO DE MEXICO | 39 | as first published, then each reform: 16 July 2002 to 17 May 2021 |
| `codigo-electoral/` | CODIGO ELECTORAL DEL ESTADO DE MEXICO | 17 | as first published, then each reform: 29 June 2014 to 4 June 2026 |
| `codigo-financiero/` | CODIGO FINANCIERO DEL ESTADO DE MEXICO Y MUNICIPIOS | 133 | as first published, then each reform: 8 April 1999 to 1 October 2026 |
| `codigo-para-la-biodiversidad/` | CODIGO PARA LA BIODIVERSIDAD DEL ESTADO DE MEXICO | 52 | as first published, then each reform: 6 May 2006 to 25 September 2026 |
| `codigo-penal/` | CODIGO PENAL DEL ESTADO DE MEXICO | 191 | as first published, then each reform: 25 March 2000 to 26 September 2026 |
| `codigo-reglamentario-del-municipio-de-toluca-2011-estado-de/` | CODIGO REGLAMENTARIO DEL MUNICIPIO DE TOLUCA 2011, ESTADO DE MEXICO | 1 | as first published: 28 June 2011 |
| `codigo-reglamentario-para-el-municipio-de-tepetlixpa-estado/` | CODIGO REGLAMENTARIO PARA EL MUNICIPIO DE TEPETLIXPA, ESTADO DE MEXICO | 1 | as first published: 10 July 2013 |
| `ley-de-acceso-de-las-mujeres-a-una-vida-libre-de-violencia/` | LEY DE ACCESO DE LAS MUJERES A UNA VIDA LIBRE DE VIOLENCIA DEL ESTADO DE MEXICO | 40 | as first published, then each reform: 21 November 2008 to 26 September 2026 |
| `ley-de-amnistia/` | LEY DE AMNISTIA DEL ESTADO DE MEXICO | 2 | as first published, then each reform: 6 January 2021 to 28 April 2026 |
| `ley-de-apicultura/` | LEY DE APICULTURA DEL ESTADO DE MEXICO | 6 | as first published, then each reform: 22 October 2014 to 6 April 2024 |
| `ley-de-apoyo-a-migrantes/` | LEY DE APOYO A MIGRANTES DEL ESTADO DE MEXICO | 4 | as first published, then each reform: 30 June 2015 to 22 November 2025 |
| `ley-de-arancel-para-el-pago-de-honorarios-de-abogados-y-cost/` | LEY DE ARANCEL PARA EL PAGO DE HONORARIOS DE ABOGADOS Y COSTAS JUDICIALES EN EL ESTADO DE MEXICO | 2 | as first published, then each reform: 8 January 1962 to 26 August 2015 |
| `ley-de-archivos-y-administracion-de-documentos/` | LEY DE ARCHIVOS Y ADMINISTRACION DE DOCUMENTOS DEL ESTADO DE MEXICO Y MUNICIPIOS | 2 | as first published, then each reform: 26 November 2021 to 1 October 2026 |
| `ley-de-asistencia-social/` | LEY DE ASISTENCIA SOCIAL DEL ESTADO DE MEXICO Y MUNICIPIOS | 9 | as first published, then each reform: 8 September 2010 to 1 November 2025 |
| `ley-de-asociaciones-publico-privadas/` | LEY DE ASOCIACIONES PUBLICO PRIVADAS DEL ESTADO DE MEXICO Y MUNICIPIOS | 2 | as first published, then each reform: 3 August 2018 to 23 June 2023 |
| `ley-de-bienes/` | LEY DE BIENES DEL ESTADO DE MEXICO Y DE SUS MUNICIPIOS | 11 | as first published, then each reform: 8 March 2000 to 18 December 2025 |
| `ley-de-bienestar-y-desarrollo-social/` | LEY DE BIENESTAR Y DESARROLLO SOCIAL DEL ESTADO DE MEXICO -ANTES- LEY DE DESARROLLO SOCIAL DEL ESTADO DE MEXICO | 19 | as first published, then each reform: 1 January 2005 to 18 December 2025 |
| `ley-de-cambio-climatico/` | LEY DE CAMBIO CLIMATICO DEL ESTADO DE MEXICO | 10 | as first published, then each reform: 22 December 2013 to 17 May 2025 |
| `ley-de-ciencia-y-tecnologia/` | LEY DE CIENCIA Y TECNOLOGIA DEL ESTADO DE MEXICO | 9 | as first published, then each reform: 31 March 2005 to 6 April 2024 |
| `ley-de-competitividad-y-ordenamiento-comercial/` | LEY DE COMPETITIVIDAD Y ORDENAMIENTO COMERCIAL DEL ESTADO DE MEXICO | 21 | as first published, then each reform: 18 March 2015 to 25 September 2026 |
| `ley-de-contratacion-publica/` | LEY DE CONTRATACION PUBLICA DEL ESTADO DE MEXICO Y MUNICIPIOS | 7 | as first published, then each reform: 30 October 2013 to 6 April 2024 |
| `ley-de-cultura-fisica-y-deporte/` | LEY DE CULTURA FISICA Y DEPORTE DEL ESTADO DE MEXICO | 7 | as first published, then each reform: 29 November 2014 to 5 February 2026 |
| `ley-de-defensoria-publica/` | LEY DE DEFENSORIA PUBLICA DEL ESTADO DE MEXICO | 14 | as first published, then each reform: 4 February 2010 to 6 April 2024 |
| `ley-de-deposito-legal/` | LEY DE DEPOSITO LEGAL PARA EL ESTADO DE MEXICO | 3 | as first published, then each reform: 14 April 2011 to 21 December 2016 |
| `ley-de-derechos-y-cultura-indigena/` | LEY DE DERECHOS Y CULTURA INDIGENA DEL ESTADO DE MEXICO | 9 | as first published, then each reform: 11 September 2002 to 6 April 2024 |
| `ley-de-educacion/` | LEY DE EDUCACION DEL ESTADO DE MEXICO | 9 | as first published, then each reform: 1 March 2024 to 17 June 2026 |
| `ley-de-eventos-publicos/` | LEY DE EVENTOS PUBLICOS DEL ESTADO DE MEXICO | 10 | as first published, then each reform: 19 August 2014 to 25 September 2026 |
| `ley-de-expropiacion/` | LEY DE EXPROPIACION PARA EL ESTADO DE MEXICO | 8 | as first published, then each reform: 18 January 1996 to 6 April 2024 |
| `ley-de-fiscalizacion-superior/` | LEY DE FISCALIZACION SUPERIOR DEL ESTADO DE MEXICO | 31 | as first published, then each reform: 29 August 2004 to 26 May 2022 |
| `ley-de-fomento-a-las-actividades-de-las-organizaciones-de-la/` | LEY DE FOMENTO A LAS ACTIVIDADES DE LAS ORGANIZACIONES DE LA SOCIEDAD CIVIL DEL ESTADO DE MEXICO | 1 | as first published: 25 May 2024 |
| `ley-de-fomento-de-la-avicultura-en-el-estado-de-mexico/` | LEY DE FOMENTO DE LA AVICULTURA EN EL ESTADO DE MEXICO | 2 | as first published, then each reform: 25 November 1956 to 5 January 1961 |
| `ley-de-fomento-de-la-cultura-de-la-legalidad/` | LEY DE FOMENTO DE LA CULTURA DE LA LEGALIDAD DEL ESTADO DE MEXICO | 3 | as first published, then each reform: 17 December 2014 to 6 April 2024 |
| `ley-de-fomento-economico/` | LEY DE FOMENTO ECONOMICO PARA EL ESTADO DE MEXICO | 25 | as first published, then each reform: 8 September 2010 to 25 September 2026 |
| `ley-de-fomento-para-la-lectura-y-el-libro/` | LEY DE FOMENTO PARA LA LECTURA Y EL LIBRO DEL ESTADO DE MEXICO | 1 | as first published: 18 December 2025 |
| `ley-de-fomento-y-proteccion-del-maiz-nativo-como-patrimonio/` | LEY DE FOMENTO Y PROTECCION DEL MAIZ NATIVO COMO PATRIMONIO BIOCULTURAL Y ALIMENTARIO DEL ESTADO DE MEXICO | 2 | as first published, then each reform: 7 October 2022 to 6 April 2024 |
| `ley-de-gobierno-de-coalicion-reglamentaria-de-los-articulos/` | LEY DE GOBIERNO DE COALICION, REGLAMENTARIA DE LOS ARTICULOS 61 FRACCION LI Y 77 FRACCION XLVIII DE LA CONSTITUCION POLITICA DEL ESTADO LIBRE Y SOBERANO DE MEXICO | 1 | as first published: 1 October 2022 |
| `ley-de-gobierno-digital/` | LEY DE GOBIERNO DIGITAL DEL ESTADO DE MEXICO Y MUNICIPIOS | 14 | as first published, then each reform: 7 January 2016 to 28 March 2026 |
| `ley-de-igualdad-de-trato-y-oportunidades-entre-mujeres-y-hom/` | LEY DE IGUALDAD DE TRATO Y OPORTUNIDADES ENTRE MUJERES Y HOMBRES DEL ESTADO DE MEXICO | 14 | as first published, then each reform: 7 September 2010 to 28 March 2026 |
| `ley-de-impuestos-sobre-el-producto-de-capitales-impuestos/` | LEY DE IMPUESTOS SOBRE EL PRODUCTO DE CAPITALES IMPUESTOS, DEL ESTADO DE MEXICO | 1 | as first published: 5 July 1930 |
| `ley-de-indulto/` | LEY DE INDULTO DEL ESTADO DE MEXICO -ANTES LEY DE INDULTO Y CONMUTACION DE PENAS DEL ESTADO DE MEXICO- | 7 | as first published, then each reform: 19 April 2016 to 6 April 2024 |
| `ley-de-ingresos-de-los-municipios/` | LEY DE INGRESOS DE LOS MUNICIPIOS DEL ESTADO DE MEXICO PARA EL EJERCICIO FISCAL 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-ingresos/` | LEY DE INGRESOS DEL ESTADO DE MEXICO PARA EL EJERCICIO FISCAL 2026 | 1 | as first published: 1 January 2026 |
| `ley-de-instituciones-de-asistencia-privada/` | LEY DE INSTITUCIONES DE ASISTENCIA PRIVADA DEL ESTADO DE MEXICO | 5 | as first published, then each reform: 13 June 2001 to 6 April 2024 |
| `ley-de-justicia-civica/` | LEY DE JUSTICIA CIVICA DEL ESTADO DE MEXICO Y SUS MUNICIPIOS | 3 | as first published, then each reform: 23 November 2023 to 17 June 2026 |
| `ley-de-justicia-cotidiana/` | LEY DE JUSTICIA COTIDIANA DEL ESTADO DE MEXICO | 3 | as first published, then each reform: 11 March 2022 to 30 April 2025 |
| `ley-de-la-comision-de-derechos-humanos/` | LEY DE LA COMISION DE DERECHOS HUMANOS DEL ESTADO DE MEXICO | 19 | as first published, then each reform: 17 August 2008 to 6 April 2024 |
| `ley-de-la-comision-de-impacto-estatal/` | LEY DE LA COMISION DE IMPACTO ESTATAL | 4 | as first published, then each reform: 6 January 2021 to 25 September 2026 |
| `ley-de-la-fiscalia-general-de-justicia/` | LEY DE LA FISCALIA GENERAL DE JUSTICIA DEL ESTADO DE MEXICO | 15 | as first published, then each reform: 10 December 2016 to 5 February 2026 |
| `ley-de-la-juventud/` | LEY DE LA JUVENTUD DEL ESTADO DE MEXICO | 14 | as first published, then each reform: 1 September 2010 to 13 March 2026 |
| `ley-de-la-universidad-autonoma/` | LEY DE LA UNIVERSIDAD AUTONOMA DEL ESTADO DE MEXICO | 4 | as first published, then each reform: 3 March 1992 to 23 June 2023 |
| `ley-de-las-personas-adultas-mayores/` | LEY DE LAS PERSONAS ADULTAS MAYORES DEL ESTADO DE MEXICO -ANTES- LEY DEL ADULTO MAYOR DEL ESTADO DE MEXICO | 9 | as first published, then each reform: 7 August 2008 to 11 April 2026 |
| `ley-de-los-cuerpos-de-bomberos/` | LEY DE LOS CUERPOS DE BOMBEROS DEL ESTADO DE MEXICO | 1 | as first published: 2 December 2021 |
| `ley-de-los-derechos-de-ninas-ninos-y-adolescentes/` | LEY DE LOS DERECHOS DE NIÑAS, NIÑOS Y ADOLESCENTES DEL ESTADO DE MEXICO | 30 | as first published, then each reform: 8 May 2015 to 21 May 2026 |
| `ley-de-mediacion-conciliacion-y-promocion-de-la-paz-social/` | LEY DE MEDIACION, CONCILIACION Y PROMOCION DE LA PAZ SOCIAL PARA EL ESTADO DE MEXICO | 5 | as first published, then each reform: 25 December 2010 to 6 April 2024 |
| `ley-de-movilidad-y-seguridad-vial/` | LEY DE MOVILIDAD Y SEGURIDAD VIAL DEL ESTADO DE MEXICO Y SUS MUNICIPIOS | 1 | as first published: 24 May 2024 |
| `ley-de-planeacion/` | LEY DE PLANEACION DEL ESTADO DE MEXICO Y MUNICIPIOS | 19 | as first published, then each reform: 24 December 2001 to 23 June 2023 |
| `ley-de-prestacion-de-servicios-para-la-atencion-cuidado-y-de/` | LEY DE PRESTACION DE SERVICIOS PARA LA ATENCION, CUIDADO Y DESARROLLO INTEGRAL INFANTIL EN EL ESTADO DE MEXICO -ANTES LEY DE CENTROS DE ATENCION, CUIDADO Y DESARROLLO INTEGRAL INFANTIL DEL ESTADO DE MEXICO- | 6 | as first published, then each reform: 6 February 2014 to 6 April 2024 |
| `ley-que-crea-al-organismo-publico-descentralizado-de-caracte/` | LEY QUE CREA AL ORGANISMO PUBLICO DESCENTRALIZADO DE CARACTER ESTATAL DENOMINADO UNIVERSIDAD TECNOLOGICA "FIDEL VELAZQUEZ" | 3 | as first published, then each reform: 30 December 1994 to 20 May 2023 |
| `ley-que-crea-el-banco-de-tejidos/` | LEY QUE CREA EL BANCO DE TEJIDOS DEL ESTADO DE MEXICO | 2 | as first published, then each reform: 7 September 2010 to 23 June 2023 |
| `ley-que-crea-el-instituto-de-verificacion-administrativa/` | LEY QUE CREA EL INSTITUTO DE VERIFICACION ADMINISTRATIVA DEL ESTADO DE MEXICO | 4 | as first published, then each reform: 18 September 2018 to 25 September 2026 |
| `ley-que-crea-el-organismo-descentralizado-denominado-institu/` | LEY QUE CREA EL ORGANISMO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE NAUCALPAN DE JUAREZ, MEXICO | 1 | as first published: 31 October 2013 |
| `ley-que-crea-el-organismo-publico-descentralizado-de-caracte/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DE CARACTER ESTATAL DENOMINADO "TECNOLOGICO DE ESTUDIOS SUPERIORES DE ECATEPEC" | 3 | as first published, then each reform: 11 September 1990 to 23 June 2023 |
| `ley-que-crea-el-organismo-publico-descentralizado-de-caracte-2/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DE CARACTER ESTATAL DENOMINADO COLEGIO DE ESTUDIOS CIENTIFICOS Y TECNOLOGICOS DEL ESTADO DE MEXICO | 5 | as first published, then each reform: 20 October 1994 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-descentralizado-de-caracte-3/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DE CARACTER ESTATAL DENOMINADO INSTITUTO MEXIQUENSE DE LA PIROTECNIA | 7 | as first published, then each reform: 16 July 2003 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-descentralizado-de-caracte-4/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DE CARACTER ESTATAL DENOMINADO INSTITUTO MEXIQUENSE DE LA VIVIENDA SOCIAL | 5 | as first published, then each reform: 24 September 2003 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-descentralizado-de-caracte-5/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DE CARACTER ESTATAL DENOMINADO TECNOLOGICO DE ESTUDIOS SUPERIORES DE COACALCO | 4 | as first published, then each reform: 5 September 1996 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-descentralizado-de-caracte-6/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DE CARACTER ESTATAL DENOMINADO UNIVERSIDAD TECNOLOGICA DE TECAMAC | 6 | as first published, then each reform: 29 June 1996 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-descentralizado-de-caracte-7/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DE CARACTER ESTATAL DENOMINADO: UNIVERSIDAD TECNOLOGICA DE NEZAHUALCOYOTL | 5 | as first published, then each reform: 8 September 1991 to 6 May 2022 |
| `ley-que-crea-el-organismo-publico-descentralizado-de-caracte-8/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DE CARACTER MUNICIPAL PARA EL MANTENIMIENTO DE VIALIDADES DE CUAUTITLAN IZCALLI | 1 | as first published: 3 July 2001 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO "INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE CHALCO", MEXICO | 1 | as first published: 26 August 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-2/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO "INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TOLUCA" | 1 | as first published: 10 September 2009 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-3/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO COLEGIO DE BACHILLERES DEL ESTADO DE MEXICO | 4 | as first published, then each reform: 29 June 1996 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-4/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO CONSEJO ESTATAL PARA EL DESARROLLO INTEGRAL DE LOS PUEBLOS INDIGENAS DEL ESTADO DE MEXICO | 5 | as first published, then each reform: 11 October 1994 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-5/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO DE FORMACION CONTINUA, PROFESIONALIZACION E INVESTIGACION DEL MAGISTERIO DEL ESTADO DE MEXICO | 2 | as first published, then each reform: 22 December 2016 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-6/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO DE LA FUNCION REGISTRAL DEL ESTADO DE MEXICO | 10 | as first published, then each reform: 2 January 2008 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-7/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE AMECAMECA, ESTADO DE MEXICO | 1 | as first published: 28 April 2011 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-8/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE AYAPANGO, ESTADO DE MEXICO | 1 | as first published: 5 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-9/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE CHICOLOAPAN, MEXICO | 1 | as first published: 5 October 2013 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-10/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE CHICONCUAC, MEXICO | 1 | as first published: 26 August 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-11/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE COACALCO DE BERRIOZABAL | 1 | as first published: 26 August 2009 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-12/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE DONATO GUERRA, MEXICO | 1 | as first published: 6 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-13/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE EL ORO, ESTADO DE MEXICO | 1 | as first published: 9 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-14/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE IXTAPALUCA | 1 | as first published: 26 August 2009 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-15/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE IXTAPAN DEL ORO, ESTADO DE MEXICO | 1 | as first published: 28 April 2011 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-16/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE JALTENCO, ESTADO DE MEXICO | 1 | as first published: 28 April 2011 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-17/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE JILOTEPEC, MEXICO | 1 | as first published: 26 August 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-18/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE JIQUIPILCO, MEXICO | 1 | as first published: 13 March 2014 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-19/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE LA PAZ, MEXICO | 1 | as first published: 26 August 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-20/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE METEPEC, ESTADO DE MEXICO | 1 | as first published: 28 April 2011 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-21/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE MORELOS, ESTADO DE MEXICO | 1 | as first published: 6 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-22/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE NEZAHUALCOYOTL, ESTADO DE MEXICO | 1 | as first published: 5 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-23/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE NOPALTEPEC, ESTADO DE MEXICO | 1 | as first published: 6 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-24/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE OTZOLOAPAN, MEXICO | 1 | as first published: 26 August 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-25/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE OTZOLOTEPEC, ESTADO DE MEXICO | 1 | as first published: 6 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-26/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE SAN JOSE DEL RINCON, MEXICO | 1 | as first published: 2 October 2013 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-27/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE SOYANIQUILPAN DE JUAREZ, MEXICO | 1 | as first published: 13 March 2014 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-28/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TECAMAC, ESTADO DE MEXICO | 1 | as first published: 17 August 2021 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-29/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TEJUPILCO, MEXICO | 1 | as first published: 2 October 2013 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-30/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TEMASCALAPA, ESTADO DE MEXICO | 1 | as first published: 6 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-31/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TEMASCALCINGO, MEXICO | 1 | as first published: 9 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-32/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TEMOAYA, MEXICO | 1 | as first published: 13 March 2014 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-33/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TENANGO DEL AIRE | 2 | as first published, then each reform: 2 August 2006 to 11 August 2011 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-34/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TEOLOYUCAN, ESTADO DE MEXICO | 1 | as first published: 6 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-35/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TEQUIXQUIAC, MEXICO | 1 | as first published: 11 August 2011 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-36/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TEZOYUCA, ESTADO DE MEXICO | 1 | as first published: 9 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-37/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TIANGUISTENCO, MEXICO | 1 | as first published: 9 October 2013 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-38/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TLALMANALCO | 1 | as first published: 26 August 2009 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-39/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TLALNEPANTLA DE BAZ, ESTADO DE MEXICO | 1 | as first published: 5 June 2025 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-40/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TLATLAYA, MEXICO | 1 | as first published: 26 August 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-41/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TULTEPEC, ESTADO DE MEXICO | 1 | as first published: 28 April 2011 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-42/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE TULTITLAN, ESTADO DE MEXICO | 1 | as first published: 6 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-43/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE VALLE DE CHALCO SOLIDARIDAD, ESTADO DE MEXICO | 1 | as first published: 9 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-44/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE VILLA DE ALLENDE, MEXICO | 2 | as first published, then each reform: 12 August 2009 to 11 August 2011 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-45/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE XONACATLAN, MEXICO | 1 | as first published: 13 March 2014 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-46/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE ZACAZONAPAN, ESTADO DE MEXICO | 1 | as first published: 9 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-47/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE CULTURA FISICA Y DEPORTE DE ZUMPANGO, ESTADO DE MEXICO | 1 | as first published: 9 November 2010 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-48/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO INSTITUTO MUNICIPAL DE LA MUJER DE TOLUCA | 1 | as first published: 4 November 2019 |
| `ley-que-crea-el-organismo-publico-descentralizado-denominado-49/` | LEY QUE CREA EL ORGANISMO PUBLICO DESCENTRALIZADO DENOMINADO SERVICIOS EDUCATIVOS INTEGRADOS AL ESTADO DE MEXICO | 3 | as first published, then each reform: 4 June 1992 to 6 April 2024 |
| `ley-que-crea-el-organismo-publico-desentralizado-denominado/` | LEY QUE CREA EL ORGANISMO PUBLICO DESENTRALIZADO DENOMINADO "INSTITUTO MUNICIPAL DE LA JUVENTUD DE AYAPANGO" | 1 | as first published: 5 August 2016 |
| `ley-que-crea-la-comision-estatal-de-seguridad-ciudadana/` | LEY QUE CREA LA COMISION ESTATAL DE SEGURIDAD CIUDADANA DEL ESTADO DE MEXICO | 3 | as first published, then each reform: 18 December 2014 to 6 September 2017 |
| `ley-que-crea-los-organismos-publicos-descentralizados-de-asi/` | LEY QUE CREA LOS ORGANISMOS PUBLICOS DESCENTRALIZADOS DE ASISTENCIA SOCIAL DE CARACTER MUNICIPAL DENOMINADO "SISTEMAS MUNICIPALES PARA EL DESARROLLO INTEGRAL DE LA FAMILIA" | 14 | as first published, then each reform: 16 July 1985 to 7 October 2022 |
| `ley-que-regula-el-regimen-de-propiedad-en-condominio-en-el-e/` | LEY QUE REGULA EL REGIMEN DE PROPIEDAD EN CONDOMINIO EN EL ESTADO DE MEXICO | 9 | as first published, then each reform: 11 July 2002 to 30 April 2024 |
| `ley-que-regula-el-uso-de-tecnologias-de-la-informacion-y-com/` | LEY QUE REGULA EL USO DE TECNOLOGIAS DE LA INFORMACION Y COMUNICACION PARA LA SEGURIDAD PUBLICA DEL ESTADO DE MEXICO | 4 | as first published, then each reform: 10 November 2014 to 6 April 2024 |
| `ley-que-regula-los-centros-de-asistencia-social-y-las-adopci/` | LEY QUE REGULA LOS CENTROS DE ASISTENCIA SOCIAL Y LAS ADOPCIONES EN EL ESTADO DE MEXICO | 11 | as first published, then each reform: 21 August 2015 to 1 May 2026 |
| `ley-que-transforma-al-organo-desconcentrado-denominado-insti/` | LEY QUE TRANSFORMA AL ORGANO DESCONCENTRADO DENOMINADO INSTITUTO DE CAPACITACION Y ADIESTRAMIENTO PARA EL TRABAJO INDUSTRIAL (I.C.A.T.I.), EN ORGANISMO DESCENTRALIZADO | 3 | as first published, then each reform: 20 August 1992 to 6 April 2024 |
| `ley-registral/` | LEY REGISTRAL PARA EL ESTADO DE MEXICO | 9 | as first published, then each reform: 2 September 2011 to 4 April 2025 |
| `ley-reglamentaria-de-las-fracciones-xxv-y-xxvi-del-articulo/` | LEY REGLAMENTARIA DE LAS FRACCIONES XXV Y XXVI DEL ARTICULO 61 DE LA CONSTITUCION POLITICA DEL ESTADO LIBRE Y SOBERANO DE MEXICO | 9 | as first published, then each reform: 4 September 2010 to 6 April 2024 |
| `ley-reglamentaria-del-articulo-88-bis-de-la-constitucion-pol/` | LEY REGLAMENTARIA DEL ARTICULO 88 BIS DE LA CONSTITUCION POLITICA DEL ESTADO LIBRE Y SOBERANO DE MEXICO | 6 | as first published, then each reform: 9 October 2004 to 6 April 2024 |
| `ley-sobre-el-escudo-y-el-himno/` | LEY SOBRE EL ESCUDO Y EL HIMNO DEL ESTADO DE MEXICO | 5 | as first published, then each reform: 2 March 1995 to 6 April 2024 |

## Source

The legislation compilation of Mexico's Supreme Court, the Suprema Corte de Justicia de la Nación (SCJN), at <https://legislacion.scjn.gob.mx/>. For each ordenamiento it lists every publication in the state's official gazette (Periódico Oficial) that changed it (decree, erratum, ruling), with the date of publication, the decree's extract and the whole consolidated text as it stood after that publication. Each version here is one of those texts.

## Dates

- Each commit is dated at **noon, America/Mexico_City, on the day the publication took effect**: the day its own transitorios name, as SCJN's extract quotes them (most often the day after publication). When a decree names none, 3 days after publication.
- A consolidated text holds every change published before it, so it is never dated before the latest of their in-force days. Different in-force days for parts of one decree are not split.
- An act's first commit is its first publication when SCJN holds the original text; otherwise it is the oldest version SCJN holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 Bis; `encabezado.md` holds the title, the promulgation and preamble; `transitorios-original.md` the original transitory articles and `transitorios-<date>.md` those of the reform published that day. Section headings and editor's notes such as "(REFORMADO, P.O. ...)" stay in the file of the article they stand before. One paragraph per line.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of SCJN's own text of that version (read independently of the parser), and every unit's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the publication that changed the text (a decree, an erratum or a ruling), named by its category, gazette date and issue, with an e-mail address that cannot exist (`<key>@legislacion.scjn.gob.mx.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one published in the state's official gazette (Periódico Oficial). The history starts with the oldest text SCJN holds for each ordenamiento, which for many is later than its enactment. Only the ordenamientos listed above are included.
