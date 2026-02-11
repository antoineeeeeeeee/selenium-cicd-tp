Analyser le rapport généré(`report.html`) :

la partie importante du rapport est la détéction d'une erreur dans le code : :

E     File "C:\Users\Rohan\Desktop\TP_GIT\selenium-cicd-tp\tests\test_selenium.py", line 13
E       @pytest.fixture(scope="class")
E       ^
E   IndentationError: expected an indented block after class definition on line 12

le problème vient de l'indentation, qui est incorrecte dans le fichier test_selenium.