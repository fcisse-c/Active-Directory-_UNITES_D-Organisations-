# Active Directory : Les Unités D'Organisations ou Unité Organisationnelle
# Documentation pour la création d'une OU, d'un groupe d'utilisateurs et d'un utilisateur dans Active Directory

## Prérequis
- Active Directory doit être installé et configuré avec le domaine `wilders.lan`.
- Vous devez être connecté en tant qu'administrateur sur le serveur Active Directory.

## Étape 1 : Créer une Unité d'Organisation (OU) `Wilders_students`

1. Ouvrez le Gestionnaire de serveur.
2. Cliquez sur **Outils** et sélectionnez **Utilisateurs et ordinateurs Active Directory**.
3. Dans la console **Utilisateurs et ordinateurs Active Directory**, faites un clic droit sur le domaine `wilders.lan` et sélectionnez **Nouveau** > **Unité d'organisation**.
4. Nommez l'Unité d'Organisation `Wilders_students` et cliquez sur **OK**.
   ![CreationUniteOrganisation](https://github.com/user-attachments/assets/90392eb9-2ee2-46d3-a60e-e2243041d3d3)


## Étape 2 : Créer un Groupe d'utilisateurs `Students`

1. Toujours dans la console **Utilisateurs et ordinateurs Active Directory**, développez le domaine `wilders.lan` et sélectionnez l'OU `Wilders_students` que vous venez de créer.
2. Faites un clic droit sur `Wilders_students`, sélectionnez **Nouveau** > **Groupe**.
3. Nommez le groupe `Students`.
4. Dans la zone **Type de groupe**, sélectionnez **Sécurité**.
5. Dans la zone **Étendue du groupe**, sélectionnez **Global**.
6. Cliquez sur **OK** pour créer le groupe.
   ![CreationGroupeAD](https://github.com/user-attachments/assets/227aae9a-4680-4f37-8c24-6016cb8db43a)


## Étape 3 : Créer un Utilisateur au sein du groupe `Students`

1. Toujours dans l'OU `Wilders_students`, faites un clic droit sur `Wilders_students`, sélectionnez **Nouveau** > **Utilisateur**.
2. Remplissez les informations de l'utilisateur :
    - **Prénom** : Sara
    - **Nom** : Doe
    - **Nom d'ouverture de session de l'utilisateur** : jdoe
3. Cliquez sur **Suivant**.
4. Saisissez le mot de passe et confirmez-le.
5. Décochez les options **L'utilisateur doit changer le mot de passe à la prochaine ouverture de session** si vous ne souhaitez pas que l'utilisateur change immédiatement son mot de passe.
6. Cliquez sur **Suivant**, puis sur **Terminer**.
 ![CreationUtilisateurAD1](https://github.com/user-attachments/assets/9261dd55-156d-4f60-bc18-a1eb879b3929)
![CreationUtilisateurAD2](https://github.com/user-attachments/assets/a077b809-31f6-4ea4-ab3a-088e351ee908)

### Ajouter l'utilisateur au groupe `Students`

1. Faites un clic droit sur l'utilisateur `John Doe` que vous venez de créer et sélectionnez **Propriétés**.
2. Allez dans l'onglet **Membre de** et cliquez sur **Ajouter**.
3. Tapez `Students` et cliquez sur **OK**.
4. Cliquez sur **Appliquer** et **OK** pour fermer la fenêtre des propriétés.

![AjoutUtilisateurGroupeAD](https://github.com/user-attachments/assets/cf9950ee-f32c-4533-b199-2ceaeb9de11c)



## Conclusion

Vous avez maintenant créé une Unité d'Organisation `Wilders_students`, un groupe d'utilisateurs `Students` et un utilisateur `John Doe` au sein de ce groupe dans Active Directory pour le domaine `wilders.lan`. 

