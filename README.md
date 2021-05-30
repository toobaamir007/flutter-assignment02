# flutter-assignment02
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        backgroundColor: Colors.grey,
        appBar: AppBar(
          title: Center(child: Text("Login Page")),
        ),
        body: Center(
          child: Column(
            children: [
              SizedBox(
                height: 50,
              ),
              Container(
                  width: 200,
                  child: TextField(
                    style: TextStyle(fontSize: 18, color: Colors.black87),
                    decoration: InputDecoration(icon: Icon(Icons.email)),
                  )),
              SizedBox(
                height: 30,
              ),
              Container(
                  width: 200,
                  child: TextField(
                    maxLength: 8,
                    style: TextStyle(color: Colors.black87),
                    obscureText: true,
                    decoration: InputDecoration(icon: Icon(Icons.lock)),
                  )),
              SizedBox(
                height: 30,
              ),
              ElevatedButton(
                onPressed: () {},
                child: Text("Login"),
              )
            ],
          ),
        ),
      ),
    );
  }
}
