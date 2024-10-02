#### Nama : Nadila Amalia Pribadi
#### Kelas: TI-3F / 19
#### NIM  : 2241720114

---

## Laporan Jobsheet 5 Pemrograman Mobile

## Praktikum 1
### - Langkah 2
![Output1](./assets/1.2.PNG)
### - Langkah 3
![Output1](./assets/1.3.PNG)
### - Langkah 4
![Output1](./assets/1.4.PNG)

## Praktikum 2
Menyambungkan dengan Emulator
![Output1](./assets/emulator.PNG)

## Praktikum 4 
### Langkah 1
```dart
import 'package:flutter/material.dart';

class MyTextWidget extends StatelessWidget {
  const MyTextWidget({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return const Text(
      "Nama saya Nadila Amalia Pribadi, sedang belajar Pemrograman Mobile",
      style: TextStyle(color: Colors.red, fontSize: 14),
      textAlign: TextAlign.center);
  }
}
```
![Output1](./assets/4.1.PNG)
### Langkah 2
```dart
import 'package:flutter/material.dart';

class MyImageWidget extends StatelessWidget {
  const MyImageWidget({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return const Image(image: AssetImage('lib/assets/logo-polinema.png'));
  }
}
```
![Output1](./assets/4.2.PNG)

## Praktikum 5
### Langkah 1
```dart
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

class LoadingCupertino extends StatelessWidget {
  LoadingCupertino({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Container(
        margin: const EdgeInsets.only(top: 30),
        color: Colors.white,
        child: Column(children: <Widget>[
          CupertinoButton(
              child: const Text('Contoh button'), onPressed: () => {}),
          const CupertinoActivityIndicator()
        ]),
      ),
    );
  }
}
```
### Langkah 2
```dart
import 'package:flutter/material.dart';

class FabWidget extends StatelessWidget {
  FabWidget({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        floatingActionButton: FloatingActionButton(
          onPressed: () => {},
          child: const Icon(Icons.thumb_up),
          backgroundColor: Colors.pink,
        ),
      ),
    );
  }
}
```
### Langkah 3
```dart
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text(widget.title),
      ),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            const Text(
              'You have pushed the button this many times:',
            ),
            Text(
              '$_counter',
              style: Theme.of(context).textTheme.headline4,
            ),
          ],
        ),
      ),
      bottomNavigationBar: BottomAppBar(
        child: Container(
          height: 50.0,
        ),
      ),
      floatingActionButton: FloatingActionButton(
        onPressed: _incrementCounter,
        tooltip: 'Increment Counter',
        child: const Icon(Icons.add),
      ), 
      floatingActionButtonLocation: FloatingActionButtonLocation.centerDocked,
    );
  }
```
![Output1](./assets/5.3.PNG)

### Langkah 3
```dart
showAlertDialog(BuildContext context) {
  // set up the button
  Widget okButton = TextButton(
    child: const Text("OK"),
    onPressed: () {
      Navigator.pop(context);
    },
  );

  // set up the AlertDialog
  AlertDialog alert = AlertDialog(
    title: const Text("My title"),
    content: const Text("This is my message."),
    actions: [
      okButton,
    ],
  );

  // show the dialog
  showDialog(
    context: context,
    builder: (BuildContext context) {
      return alert;
    },
  );
}
```
![Output1](./assets/5.4.PNG)

### Langkah 4
```dart
class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(title: const Text("Contoh TextField")),
        body: const TextField(
          obscureText: false,
          decoration: InputDecoration(
            border: OutlineInputBorder(),
            labelText: 'Nama',
          ),
        ),
      ),
    );
  }
}
```
![Output1](./assets/5.5.PNG)

### Langkah 5
```dart
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text(widget.title),
      ),
      body: Center(
        child: Column(
          mainAxisSize: MainAxisSize.min,
          children: <Widget>[
            Text("${selectedDate.toLocal()}".split(' ')[0]),
            const SizedBox(
              height: 20.0,
            ),
            ElevatedButton(
              onPressed: () => {
                _selectDate(context),
                // ignore: avoid_print
                print(selectedDate.day + selectedDate.month + selectedDate.year)
              },
              child: const Text('Pilih Tanggal'),
            ),
          ],
        ),
      ),
    );
  }
```
![Output1](./assets/5.6.PNG)

# Tugas Praktikum Codelabs Google
### Langkah 3
![Output1](./assets/tp2.PNG)

### Langkah 4
![Output1](./assets/tp4.PNG)

### Langkah 5
![Output1](./assets/tp5.PNG)
![Output1](./assets/tp6.PNG)
![Output1](./assets/tp7.PNG)
![Output1](./assets/tp8.PNG)
![Output1](./assets/tp9.PNG)
![Output1](./assets/tp10.PNG)

### Langkah 6
![Output1](./assets/tp13.PNG)

### Langkah 7
![Output1](./assets/tp14.PNG)
![Output1](./assets/tp15.PNG)
![Output1](./assets/tp16.PNG)
![Output1](./assets/tp17.PNG)

### Langkah 8
![Output1](./assets/tp18.PNG)
![Output1](./assets/tp19.PNG)


