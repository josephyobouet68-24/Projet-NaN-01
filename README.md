# Projet-NaN-01
Projet NaN 01


## EXERCICE1  NOMBRE MYSTÈRE

'''php
 
    function nombreMysterieux($SaisirUser = 0)
    {

        // Default answer value
        $answer = "Veuillez saisir un nombre.";

        if (! empty($SaisirUser)) 
        {   
            // Initialiser les variables
            $nombreMystere  = rand(1,99);

            // Obtenir le nombre saisi par l'utilisateur
            $SaisirUtilisateur = (! empty($SaisirUser) && intval($SaisirUser) < 100 ) ? intval($SaisirUser) : 0 ;

            if ($nombreMystere === $SaisirUtilisateur) 
            {
                $answer = "Vous avez gagné ! ";
            }//Fin si 
            elseif ($nombreMystere < $SaisirUtilisateur) 
            {
                $answer = "Le nombre est trop grand !";

            }//Fin sinon si
            else 
            {
                // $result = "Le nombre mystère est plus petit !";
                $answer ="Le nombre est trop petit !";

            }//Fin sinon
                
        }// Fin si

        // Return value
        return $answer;

    }// Fin de la fonction
    
'''

 ## EXERCICE2 FONCTION PURGE
 
 '''php
 
    function FonctionPurge($Phrase = '', $MotPurge = '')
    {
        // Obtenir la saisie de l'utilisateur
        $PhraseUtilisateur = (! empty($Phrase) && is_string($Phrase)) ? ($Phrase) : '' ;

        // Obtenir la lettre ou le caractère à supprimer
        $MotPurgeUtilisateur = (! empty($MotPurge) && is_string($MotPurge)) ? ($MotPurge) : '' ;

        // Traiter uniquement s'il y a des données disponibles.
        if (! empty($PhraseUtilisateur) && ! empty($MotPurgeUtilisateur)) 
        {   
            
             $answer = str_replace($MotPurgeUtilisateur, '', $PhraseUtilisateur);

            
        }//Fin si

        // Return value
        return $answer;

    }// Fin de la fonction
    
'''
