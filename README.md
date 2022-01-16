# naija_uni

Returns a list of universities in Nigeria and can be used anywhere.

## Drop Down
it can be used in a dropdown to prompt easy selection

```dart
DropdownButton(
            items: NaijaUni.allUniversities.map((String value) {
              return DropdownMenuItem<String>(
                value: value,
                child: Text(value),
              );
            }).toList(),
            onChanged: (_) {},
          ),
```

## ListView
can be used in a list view to display all universities

```dart
ListView.builder(
              itemCount: NaijaUni.allUniversities.length,
              itemBuilder: (context, index) {
                String university = NaijaUni.allUniversities[index];
                return Container(
                  child: Text(university),
                );
              }),
```

