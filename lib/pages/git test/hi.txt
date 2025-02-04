import 'package:flutter/material.dart';

class Home extends StatelessWidget {
  const Home({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Row(
          mainAxisAlignment: MainAxisAlignment.spaceBetween,
          children: [
            Column(
              crossAxisAlignment: CrossAxisAlignment.start,
              children: [
                Text(
                  "Hello, Welcome",
                  style: TextStyle(
                    fontSize: 20,
                    fontWeight: FontWeight.w200,
                  ),
                ),
                Text(
                  "Alex Sharma",
                  style: TextStyle(
                    fontSize: 26,
                    fontWeight: FontWeight.w500,
                  ),
                ),
              ],
            ),
            CircleAvatar(
              backgroundImage: AssetImage('assets/images/img-1.jpg'),
            )
          ],
        ),
      ),
      body: Padding(
        padding: const EdgeInsets.fromLTRB(10.0, 10, 10, 0),
        child: Center(
          child: SingleChildScrollView(
            // scrollDirection: Axis.vertical,      //default
            child: Column(
              children: [
                SizedBox(
                  height: 40,
                ),
                Text(
                  'vitra.',
                  style: TextStyle(
                    fontWeight: FontWeight.w900,
                    fontSize: 40,
                  ),
                ),
                SizedBox(
                  height: 25,
                ),
                Text(
                  'Products',
                  style: TextStyle(
                    fontWeight: FontWeight.w200,
                  ),
                ),
                SizedBox(
                  height: 16,
                ),

                //images
                ListView(
                  children: [
                    Text('data'),
                    Text('data'),
                    Text('data'),
                  ],
                )
              ],
            ),
          ),
        ),
      ),
    );
  }
}
