# SAP-ERP-system-for-inventory-management-system-ABAP
ABAP notes which helpful to develope this project.
sap report
obligatory - use to select option field where if we didn't enter input data then show error .
select option- search karva mate nu khanu bane.
initialization- value khana ma bydefault bhareli re. fenil-low ""  fenil-high "" range declare karvani. append fenil. karvanu atle value tya jay.
AT SELECTION-SCREEN - input field na data ne verify kare khali hoy to message batave.if elseif endif statement ma message batavana.
top-of-page - attribute na name. end-of-page.

start of selection // end of selction - query and loop bane chale .

programme name zperform_10
perform function_name() ama value return karavani - USING num1 num2 CHANGING sum.
Form function_name() ama logic banavanu .. 
perform ma declare karela variable form ma chale pan form na variable perform ma ni chale

 
Hide option  (4)
At line selection. (5)


alv containt......
workflow - wf  (6)
tableflow - Tf  (7)  alv
CALL FUNCTION 'REUSE_ALV_GRID_DISPLAY' 
TF TYPE SLIS_T_FIELDCAT_ALV,
WF TYPE SLIS_FIELDCAT_ALV.

alc intractive use thay.............
FORM FENIL USING SK LIKE SY-UCOMM RS_SELFIELD TYPE SLIS_SELFIELD.
    CASE SK.
      WHEN '&IC1'.
        READ TABLE IT2 INTO WA2 INDEX RS_SELFIELD-TABINDEX.
