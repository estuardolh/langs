# Pascal

Expressions
```pascal
{ vars }
var_name : type;
pointer_var_name : ^type;

var_name := value;
pointer_var_name = @type;

{ array length }
Length( an_array )

{ out, in }
write( arg );
writeln( arg );
readln;
```

Operators
```pascal
<>  { not equals }
:= { assignation }
```

statements
```pascal
  for i := 0 to n do
  begin
    { logic here }
  end;

  if 0 < 10 then
    write('text  ') { no ';' before else }
  else
  begin
    { else logic here }
  end;

  if 2 mod 0 = 1 then
  begin
    { nested if }
    if 2 mod 0 = 0 then
    begin
      { logic here }
    end;
  end;
```

Classes / units
```pascal
unit a_unit;

interface

uses crt; { units to use }

const
  a_const = 1; { const declaration & definition }

type
  { public declarations here }

{ implementation here }

end.
```

Records
```pascal
  a_record = Record
               { vars declaration here }
             end;
```

Array declarations
```pascal
  an_array = Array[0..10] of a_record;
```

Procedure & function declaration
```pascal
  procedure a_proc( var a_var: a_type );
  function a_function( a_var1 : a_type1 ; a_var2 : a_type2 ) : Integer;
```

Proc. definition
```pascal
procedure a_proc( var a_var: a_type );
var
  { local var declaration here }
begin
  { logic here }
end;
```
Func. definition
```pascal
function a_function( a_var1 : a_type1 ; a_var2 : a_type2 ) : Integer;
var
  { local var declaration here }
begin
  a_function := 2; { value to return }
end;
```