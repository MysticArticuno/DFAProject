For the GUI version go to the InterfaceDFA folder
For a version that is runnable in the command line go to the DFAProject folder

If you are running InterfaceDFA from the command line, include the following jvm arguments:
--module-path "./javafx/lib" --add-modules javafx.controls,javafx.fxml

I was able to fix the issue I was encountering during the presentation by switching from Scanner.next() to Scanner.nextLine()
the next() function stops reading the String if it encounters a space, and my project directory had a space in it.