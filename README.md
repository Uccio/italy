# italy

Questo modulo per Drupal 7 crea le strutture dati necessarie a contenere le provincie e le regioni italiane all'interno di Drupal ed espone alcune funzioni utili alla creazione di form specifici per l'italia.
Alcuni esempi di come utilizzare le funzioni all'interno del modulo per creare dei form tipicamente italiani:

       $form['provincia'] = array(
          '#weight' => 5,
          '#type' => 'select',
          '#options' =>italy_ListProvince(),
          '#title' => t('Provincia'),
          '#empty_value' => '',
          );
        
        $form['regione'] = array(
          '#weight' => 5,
          '#type' => 'select',
          '#empty_value' => '',
          '#options' =>italy_ListRegioni(),
          '#title' => t('Regione'),
        );


Rigraziamenti:
- rickystra per i dati: https://github.com/rickystra/Regioni-province-comuni
