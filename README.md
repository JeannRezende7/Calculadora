# Calculadora
Calculadora Simples que pode ser feita com com if ou Switch

 ````
 var n1, n2: double;
  var x: Char;
begin
  n1:= strToFloat(lb_num1.Text);
  n2:= strToFloat(lb_num2.Text);
  
//utilização do switch
  x := lb_operador.Text[1];
   case x of

       '+' : 
        begin
            ShowMessage (FloatToStr(n1 + n2));
        end;

        '-' : 
        begin
            ShowMessage (FloatToStr(n1 - n2));
        end;

        'x' : 
        begin
            ShowMessage (FloatToStr(n1 * n2));
        end;

        '/' : 
        begin
            ShowMessage (FloatToStr(n1 / n2));
        end;
   end;
 ````
    
   ````
   //efetuando pelo if
  if(lb_operador.Text = '+') Then
  begin
      ShowMessage (FloatToStr(n1 + n2));
  end;
  //efetuando a subtração
  if(lb_operador.Text = '-') Then
  begin
      ShowMessage (FloatToStr(n1 - n2));
  end;
  //efetuando a multiplicação
  if(lb_operador.Text = 'x') Then
  begin
      ShowMessage (FloatToStr(n1 * n2));
  end;
  //efetuando a divisão
  if(lb_operador.Text = '/') Then
  begin
      ShowMessage (FloatToStr(n1 / n2));
  end;   
  ````
