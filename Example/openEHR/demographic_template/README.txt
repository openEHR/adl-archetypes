

	This example illustrates the design of a realistic template based on the openEHR demographic model.
	
	The root template, openEHR-DEMOGRAPHIC-PERSON.t_patient_simple.v1 specialises the archetype 
	openEHR-DEMOGRAPHIC-PERSON.person.v1 by choosing slot fillers for 3 slots, found at the 
	/details[at0001]/items, /identities, /contacts[at0003]/addresses paths. Each of these slots
	is also closed, preventing further additions either in more specialised templates, or at 
	runtime.

	Each of the slot filler template components removes various unneeded data items from the original
	parent archetypes, leaving only those needed for the template. You can see what each template
	component removes by exploring in the template structure (lower left hand of ADL Workbench), and
	using the Differential View tab, and '+ class names' RM visibility setting on the right. Use the 
	Flat View tab to show the result of the removals.

