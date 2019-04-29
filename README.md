<h2>SQL Oracle</h2>
<p>Reposit&oacute;rio destinado a manter e disponibilizar queries e scripts SQL que possam ajudar no dia a dia</p>

<p>Consulta para identificar campos no banco de dados Oracle:</p>
<div class="highlight highlight-source-shell"><pre> 
SELECT *
  FROM all_tab_columns
 WHERE upper(column_name)  LIKE '%TIPO_VALOR%'
 ORDER BY OWNER, TABLE_NAME
 
</pre></div>


<p>Chamada de Procedure via SQL Editor com passagem de Parâmetros:</p>
<div class="highlight highlight-source-shell"><pre> 
DECLARE
  p_mes_referencia varchar2(10);

BEGIN
  -- Call the procedure
  p_mes_referencia := '31/03/2019';  
  ts.nome_procedure(p_mes_referencia);
  
END;

</pre></div>
