# Algorithm
- Start by reading the four entities by its path (for example 'curateddata/Collections.csv') and assign them to variables called artworks, creators, exhibitions & collections. 
- Read the relationships between the entities and assign it to variables. 
- Create the empty table called filtered_exhibitions that is filled by the algorithm.
- Enter a date and assign it to a variable called selected_date.
- While(there is exhibitions left in the exhibitions table)
	Get the next exhibition
	If(exhibition.start_date == entered date)
		Put the exhibition in the list filtered_exhibitions
		Show the list of selected exhibitions to choose from
		While(the list of selected exhibitions has exhibitions left) 
			Get all of its art 
			While(it has art left)	 
				Get all of its creators. 
                Select a gender of the availiable genders and assign it to a variable called selected_gender. 
				While(it has creators left) 
					Check the gender of the creator against selected_gender
					If(the gender is the selected) 
					    Bring only the art by a creator of the selected gender connected to that exhibition 
					EndIf;  
				EndWhile;
			EndWhile; 
		EndWhile; 
		Return the list of exhibitions together with its art and creator  
	Else
		Print that there are no exhibitions during the selected year and return to enter a date. 
	Endif; 
- Endwhile; 