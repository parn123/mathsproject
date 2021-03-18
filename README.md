----------------------------------------------------------------------sin (x)----------------------------------------------------------------------------------------

>> syms x
>> f=sin(x);
>> taylor2=taylor(sin(x),x,pi/2,'order',2);
>> taylor4=taylor(sin(x),x,pi/2,'order',4);
>> taylor6=taylor(sin(x),x,pi/2,'order',6);
>> taylor8=taylor(sin(x),x,pi/2,'order',8);
>> taylor10=taylor(sin(x),x,pi/2,'order',10);
>> fplot([taylor2 taylor4 taylor6 taylor8 taylor10 f])
>> grid on
>> xlim([-4,7])
>> ylim([-4,4])
>> legend('degree 0', 'degree 2', 'degree 4', 'degree 6', 'degree 8','sin(x)')

---------------------------------------------------------------------  log (x) ------------------------------------------------------------------------------------

>> syms x
>> f=log(x);
>> taylor2=taylor(log(x),x,exp(1),'order',2);
>> taylor4=taylor(log(x),x,exp(1),'order',4);
>> taylor6=taylor(log(x),x,exp(1),'order',6);
>> taylor8=taylor(log(x),x,exp(1),'order',8);
>> taylor10=taylor(log(x),x,exp(1),'order',10);
>> fplot([taylor2 taylor4 taylor6 taylor8 taylor10 f])
>> grid on
>> xlim([-2,5])
>> ylim([-4,4])
>> legend('degree 1', 'degree 3', 'degree 5', 'degree 7', 'degree 9','log(x)')

------------------------------------------------------------------ sin(x)/x --------------------------------------------------------------------------------------

>> syms x
>> f=sin(x)/x;
>> taylor2=taylor(sin(x)/x,x,0,'order',2);
>> taylor4=taylor(sin(x)/x,x,0,'order',4);
>> taylor6=taylor(sin(x)/x,x,0,'order',6);
>> taylor8=taylor(sin(x)/x,x,0,'order',8);
>> taylor10=taylor(sin(x)/x,x,0,'order',10);
>> fplot([taylor2 taylor4 taylor6 taylor8 taylor10 f])
>> grid on
>> xlim([-8,8])
>> ylim([-4,4])
>> legend('degree 0', 'degree 2', 'degree 4', 'degree 6', 'degree 8', 'sinx/x')

--------------------------------------------------------------------  e^x  ------------------------------------------------------------------------------------------
>> syms x
>> f=exp(x);
>> taylor2=taylor(exp(x),x,1,'order',2);
>> taylor4=taylor(exp(x),x,1,'order',4);
>> taylor6=taylor(exp(x),x,1,'order',6);
>> taylor8=taylor(exp(x),x,1,'order',8);
>> taylor10=taylor(exp(x),x,1,'order',10);
>> fplot([taylor2 taylor4 taylor6 taylor8 taylor10 f])
>> grid on
>> xlim([-8,4])
>> ylim([-10,10])
>> legend('degree 1', 'degree 3', 'degree 5', 'degree 7', 'degree 9', 'e^x')

-------------------------------------------------------------------- tan inverse x ------------------------------------------------------------------------------------

>> syms x
>> f=atan(x);
>> taylor2=taylor(atan(x),x,1,'order',2);
>> taylor4=taylor(atan(x),x,1,'order',4);
>> taylor6=taylor(atan(x),x,1,'order',6);
>> taylor8=taylor(atan(x),x,1,'order',8);
>> taylor10=taylor(atan(x),x,1,'order',10);
>> fplot([taylor2 taylor4 taylor6 taylor8 taylor10 f])
>> grid on
>> xlim([-10,10])
>> ylim([-6,6])
>> legend('degree 1', 'degree 3', 'degree 5', 'degree 7', 'degree 9', 'tan inverse x')

------------------------------------------------------------------------------------------------------------------------------------------------------------------------
