# linhas-ctrlC-CTRLv
Salvar Algumas Linhas do Projeto.






var nome=addForm.nome.value;
    var peso=addForm.peso.value;
    var altura=addForm.altura.value;
    var gordura=addForm.gordura.value;

    var paciente=document.createElement(`tr`);

    var nomeTd=document.createElement(`td`);
    var pesoTd=document.createElement(`td`);
    var alturaTd=document.createElement(`td`);
    var gorduraTd=document.createElement(`td`);
    var imcTd=document.createElement(`td`);


    nomeTd.textContent=nome;
    pesoTd.textContent=peso;
    alturaTd.textContent=altura;
    gorduraTd.textContent=gordura;
    imcTd.textContent=calculaImc(peso, altura);



    paciente.appendChild(nomeTd);
    paciente.appendChild(pesoTd);
    paciente.appendChild(alturaTd);
    paciente.appendChild(gorduraTd);
    paciente.appendChild(imcTd);




    var tabela= document.querySelector("#tabela-pacientes");

    tabela.appendChild(paciente);

