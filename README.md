# TurinMachine-cpp
Maquina de turing:

Para Σ = {a,b}, a Máquina de Turing que aceita a linguagem L = {a^nb^n}|n ≥ 1} pode ser definida como: 
M = ({q0,q1,q2,q3,q4}, {a,b}, {a,b,x,y,Z(vazio)}, qo, {q4}, δ) com:

δ(q0,a) = (q1,x,R), 
δ(q1,a) = (q1,a,R), 
δ(q1,y) = (q1,y,R), 
δ(q1,b) = (q2,y,L), 
δ(q2,y) = (q2,y,L), 
δ(q2,a) = (q2,a,L), 
δ(q2,x) = (q0,x,R) 
δ(q0,y) = (q3,y,R), 
δ(q3,y) = (q3,y,R), 
δ(q3,Z) = (q4, Z,R)
