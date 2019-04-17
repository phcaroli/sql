<h2>SQL Oracle</h2>
<p>Reposit&oacute;rio destinado a manter e disponibilizar queries e scripts SQL que possam ajudar no dia a dia</p>

<li>Consulta para identificar campos no banco de dados Oracle:</li>

<div class="highlight highlight-source-shell"><pre> 
SELECT *
  FROM all_tab_columns
 WHERE upper(column_name)  LIKE '%TIPO_VALOR%'
 ORDER BY OWNER, TABLE_NAME
 
</pre></div>
