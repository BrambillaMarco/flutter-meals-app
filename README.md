# 🍽️ Meals App

Un’app Flutter per esplorare ricette, filtrare i pasti in base a preferenze alimentari e gestire una lista di preferiti.  
Il progetto dimostra l’uso di **Riverpod** per la gestione dello stato, animazioni di base, `Hero` widgets, e la strutturazione modulare del codice.

---

## Funzionalità

- **Categorie di pasti**: esplora piatti suddivisi per tipologia (italiana, asiatica, vegetariana, ecc.).  
- **Filtri personalizzati**: scegli se visualizzare solo ricette **senza glutine, senza lattosio, vegetariane o vegane**.  
- **Preferiti**: aggiungi o rimuovi pasti dalla tua lista personale di preferiti.  
- **Animazioni fluide**:  
  - transizioni con `Hero` per le immagini,  
  - `AnimatedSwitcher` per lo stato dei preferiti,  
  - `SlideTransition` per l’ingresso delle categorie.  
- **UI moderna**: tema scuro con **Material 3** e font **Google Fonts (Lato)**.  

---

## Tecnologie utilizzate

- [Flutter](https://flutter.dev/)
  
- [Riverpod](https://riverpod.dev/) — gestione dello stato reattivo
  
- [Google Fonts](https://pub.dev/packages/google_fonts)
  
- [transparent_image](https://pub.dev/packages/transparent_image)
  

---

## 📂 Struttura del progetto

lib/

├── main.dart # Entry point con tema e MaterialApp

├── data/

│ └── dummy_data.dart # Dati fittizi (categorie e pasti)

├── models/

│ ├── category.dart # Modello Categoria

│ └── meal.dart # Modello Meal

├── providers/

│ ├── meals_provider.dart

│ ├── filters_provider.dart

│ └── favorites_provider.dart

├── screens/

│ ├── tabs.dart # Navigazione principale con BottomNavigationBar

│ ├── categories.dart # Griglia categorie

│ ├── meals.dart # Lista pasti

│ ├── meal_details.dart # Dettaglio di un pasto

│ └── filters.dart # Filtri alimentari

└── widgets/

├── main_drawer.dart # Drawer laterale

├── category_grid_item.dart

├── meal_item.dart

└── meal_item_trait.dart

---

## Avvio del progetto

1. Clona il repository  
   ```bash
   git clone https://github.com/BrambillaMarco/flutter-meals-app.git
   
2. Entra nella cartella del progetto
cd meals-app

3. Installa le dipendenze
flutter pub get

4. Avvia l’app su un emulatore o dispositivo
flutter run

---

## Screenshots

<img width="1124" height="708" alt="screen-meals-app" src="https://github.com/user-attachments/assets/3446a973-ff8e-4e61-8e87-cda13dfb7227" />

<img width="1047" height="708" alt="screen2-meals-app" src="https://github.com/user-attachments/assets/93648821-d5a2-4c6b-9077-21fd515f7fc4" />

<img width="711" height="737" alt="screen3-meals-app" src="https://github.com/user-attachments/assets/b044b4a7-d4fd-48f2-851f-c592517389a5" />

---

## Cosa ho imparato
-Durante lo sviluppo di questa app ho acquisito esperienza pratica con:

-gestione dello stato con Riverpod, inclusi StateNotifier e Provider.

-uso di animazioni personalizzate (AnimationController, SlideTransition, RotationTransition).

-uso di animazioni preconfigurate (AnimatedSwitcher, FadeInImage, Hero).

-costruzione di widget riutilizzabili e modulari (CategoryGridItem, MealItem, MealItemTrait).

-implementazione di drawer laterale e navigazione tra schermate con Navigator.

-filtraggio dinamico di dati in base a preferenze utente.

-creazione di interfaccia moderna con tema scuro.

-gestione di liste e griglie in Flutter (ListView.builder, GridView).

-transizioni fluide tra pagine e gestione dello stato dei preferiti con notifiche utente (SnackBar).
