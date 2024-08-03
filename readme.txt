

Skill use for this project 
	Java Swing -(GUI)
	Java's java.net.Socket class represents a socket, and
		it allows Java applications to communicate over the
		network in a platform-independent manner.
		
	Socket-for bi-directional communication between two networked applications.
		They are associated with a specific port number,
		allowing the TCP protocol to determine the intended
		recipient application for the data\
	
	ServerSocket: These are designed to listen for incoming network requests, 
		execute an action based on the request, and potentially send a
		response back to the requester.
		
		
		
	ChatServer.java (server)- 
		Instantiate a ServerSocket, assigning it a specific port to monitor 
			for incoming requests.
		Use the ServerSocket's accept() method to await a client's connection, 
			which halts execution until a connection is established. 
		After accepting a connection, the server can interact with the client 
			using the Socket object that the accept() method provides.
			
			
	ChatClient.java (Client)
		Initialize a Socket object with the server's hostname and port number 
			to establish a connection.
		After the connection is successfully established, the client can use 
		the Socket object to communicate with the server.
	
	ChatGlientGUI.java (user UI)
		graphical user interface (GUI) for our chat client using Java Swing.
		
		extending JFrame to provide a basic window for your application and using a JTextArea for
			displaying messages and a JTextField for typing new messages.
		user input, we’ll have an action listener for the textField and this will be looking
			for when the user presses Enter.
			
	to RUN
	javac