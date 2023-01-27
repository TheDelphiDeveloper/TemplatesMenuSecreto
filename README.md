# TemplatesMenuSecreto

Como criar um template para Delphi (Post Menu Secreto)
```xml
<?xml version="1.0" encoding="utf-8" ?>
<codetemplate	xmlns="http://schemas.borland.com/Delphi/2005/codetemplates"
				version="1.0.0">
  
  ///name = a tag que vai digitar dentro do seu codigo e apertar Tab  
	<template name="MinhaQuery" invoke="manual">  
		<description>  ///Coloque uma descrição para que serve este template
          Estrutura Prontas para Insert
		</description>
    
    ///Coloque o autor (seu nome)
		<author>
           The Delphi Developer
		</author> 
    
    ///coloque language Delphi e seu código que quer que apareca tem de ficar dentro de '<![CDATA[ aqui dentro ]]>'    
		<code language="Delphi"><![CDATA[var SQLQuery1 := TSQLQuery.Create(Nil);
  try
    SQLQuery1.SQLConnection := ;
    SQLQuery1.SQL.Clear;
    SQLQuery1.SQL.Text('INSERT INTO TABLE() VALUES ();');
    SQLQuery1.ExecSQL;
    SQLQuery1.Close;
  finally
    SQLQuery1.Free;
  end;]]>
		</code>
	</template>
</codetemplate>

```
