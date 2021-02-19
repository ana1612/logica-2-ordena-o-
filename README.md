# logica-2-ordena-o-
1
packageordenação_lg2 ;
	

	classe pública Ordena ção_1 {
	

		publicstaticvoidmain ( String [] args ) {
			
			vetor int [] = { 3 , 6 , 2 , 1 , 8 , 4 };
			intaux;
			controle booleano ;
			
			para ( int i = 0 ; i < vetor . comprimento; ++ i) {
				controle = verdadeiro ;
				for ( int j = 0 ; j < (vetor . comprimento - 1 ); ++ j) {
					
					se (vetor [j] > vetor [j + 1 ]) {
						aux= vetor [j];
						vetor [j] = vetor [j + 1 ];
						vetor [j + 1 ] =aux;
						controle = falso ;
					}
					
				}
					
					if (controle) {
						pausa ;
					}
				}
			
			para ( int i = 0 ; i < vetor . comprimento; ++ i) {
				Sistema . para fora . println (vetor [i] + " " );	
			}
		
	

		}
	

	}
2
packageordenação_lg2 ;
	

	importjava.util.Arrays ;
	importjava.util.Random ;
	

	classe pública Ordena ção_2 {
	

		publicstaticvoidmain ( String [] args ) {
			
			int [] v =gerarVetor ( 10 );
			selectionSort (v);
			Sistema . para fora . println ( Arrays.toString (v));
		}
		
		privatestaticvoidselectionSort ( int [] v ) {
			para ( int i = 0 ; i < v . comprimento; i ++ ) {
				int menor = i;
				para ( int j = i + 1 ; j < v . comprimento; j ++ ) {
					if (v [j] < v [menor])
						menor = j;
				}
				
				trocar (v, i, menor);
			}
		}
		
		trocarteprivado estático vazio  ( int [] v , inti , intmenor ) {  
			intaux= v [i];
			v [i] = v [menor];
			v [menor] =aux;
		}
	

		publicstaticint [] gerarVetor ( intn ) {
		int [] v = novo int [n];
		Gerador aleatório = novo Random ();
		para ( int i = 0 ; i < n; i ++ ) {
			v [i] = gerador . nextInt ( 100 );
		}
		return v;
		}
	}

3 

packageordenação_lg2 ;
	

	publicclassRecursão {
			
			publicstaticintfatorialNaoRecursivo ( intnum ) {
				
				if (num == 0 ) {
					return1 ;
				}
				
				total int = 1 ;
				para ( int i = num; i >1 ; i - ) {
					total * = i;
				}
				
				retorno total;
			}
			
			publicstaticintfatorial ( intnum ) {
				
				if (num == 0 ) {
					return1 ;
				}
				
				retornar num * fatorial (num - 1 );
			}
	

		}
	

