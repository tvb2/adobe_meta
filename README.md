# adobe_meta
edit pdf meta information (pet project)
To do:
 - change the way created and modified date are parsed: currently we are looking for '/CreateDate (D:' tag for new style pdf, but need to look for '/CreateDate' and allow for space(s) before '(D:'
 - change the way we handle cases when user presses 'Updte' button more than once.
 - Add a pop up message to notify that changes have been successfully made and add file name
 - only display as Found fields if meta data exists in pdf (like 'modified' date). If it wasn't found, do not display the field and do not allow user to 'update' these fields
