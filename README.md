Analyser le rapport généré(`report.html`) :

la partie importante du rapport est la détéction d'une erreur dans le code : :

E     File "C:\Users\Rohan\Desktop\TP_GIT\selenium-cicd-tp\tests\test_selenium.py", line 13
E       @pytest.fixture(scope="class")
E       ^
E   IndentationError: expected an indented block after class definition on line 12

le problème vient de l'indentation, qui est incorrecte dans le fichier test_selenium.



Quels sont les avantages de l’automatisation des tests que vous avez constatés ?

L’automatisation permet de vérifier rapidement que les fonctionnalités principales fonctionnent toujours après une modification. Elle fait gagner du temps par rapport aux tests manuels et réduit les erreurs humaines. Elle permet aussi de détecter immédiatement les régressions.

Comment le CI/CD améliore-t-il la qualité du code ?

Le CI/CD exécute automatiquement les tests à chaque push ou pull request, ce qui évite d’intégrer une régression. Il garantit que le projet fonctionne dans un environnement propre et standardisé.

Quelles difficultés avez-vous rencontrées avec Selenium ?

Les principaux problèmes concernent le temps de chargement des pages et les éléments parfois non détectés au bon moment. Il peut aussi y avoir des soucis de compatibilité entre versions de navigateur et de driver. Les tests peuvent devenir instables si les attentes ne sont pas bien configurées.

Comment pourriez-vous améliorer la stabilité des tests ?

On peut utiliser des attentes explicites (WebDriverWait) plutôt que des time.sleep. Il faut avoir un environnement de test stable et cohérent.

Quelles métriques sont les plus importantes pour votre projet ?

Le taux de réussite des tests, la couverture de code et le temps d’exécution du pipeline sont essentiels. Ces indicateurs permettent de mesurer la qualité et la performance du projet. La stabilité des tests est également une métrique importante.

Comment mesurer l’efficacité de votre pipeline CI/CD ?

On peut analyser le nombre d’échecs détectés avant mise en production et la rapidité des retours. Le temps moyen d’exécution et la fréquence des builds réussis sont aussi des indicateurs clés.