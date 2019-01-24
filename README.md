# DOCTOR-X

done using Flutter

In medical field one common problem faced by people is to deal with big list of medical tests
even when not needed which increases the cost of treatment. This is mainly because of
doctor’s inability of predict exact disease. Another problem is patient’s negligence towards
some simple symptoms which may potentially a serious health issue, but the refrain from
going to doctor fearing of spending thousands on medical tests and outcome being some
simple heath issue or none at all.

Our idea is to make the task of predicting a disease easier for doctor and give a virtual
doctor to every person with which he can share his symptoms and get to know probable
health issue and should he actually visit a doctor.

We will have a user interface which takes input as person’s age, gender, weight, physical
body symptoms and psychological symptoms. Using artificial neural network we train a
model which takes medical data like symptoms and age as features and diseases as output.
If probability of two disease is very close as computed by model then it will suggest a
medical test on one of the diseases to confirm. After the model performs satisfactorily on
training set we can go for real world implementations by adding more features to
application like :-

### Tech

virtual doctor uses a number of open source projects to work properly:
Flutter :To build a user interface an take input of symptoms from user
Neural Network : A machine learning approach to predict disease
Dataset : to train the model

### Installation
Doctor X has been programmed in flutter

install flutter
Install Android studio


### Development

# doctorx

A new Flutter application.

## Creating the frontend to take user input
    ##first we create a dropdown button to take in "body condition" type of symptoms

                            DropdownButton<String>(
                                    hint: Text("Body Conditions"),
                                           items: <String>[
                                             'Loose Motions',
                                             'Rashes',
                                             'Vomiting',
                                             'Loss of appetite',
                                             'Skin Wrinkling',
                                             'Dry mucus',
                                             'Coughing',
                                             'Too much Thirst',
                                             'Yello Eye',
                                             'Yellow Skin',
                                             'Yellow Urine',
                                             'Itching',
                                             'Weight Loss',
                                             'Pox',
'

            Similarly 3 more drop downs namely physical pains" "psychological conditions" and "fever range" is created

    ##then we create a floating ction button to add new dropdown field if user want to enter more symptoms
                             FloatingActionButton(onPressed: () {},child: Icon(Icons.add),)


    ##We also need a parameter to judge how confident a user is about his symptom which in terms give us probability of the the symptom to be present in the patient.
                (in bayesian learing approach this gives us prior probability of occurance of an event)

                                  Spacer(),StarRating(size: 25,rating: rating2,onRatingChanged: (rt){
                                          setState(() {
                                            rating2=rt;

    ##and finally a submittion button and a field to show final output
                             SizedBox(
                                     height: 20,
                                        ),
                                      Center(child: FloatingActionButton(child: Icon(Icons.done),)),
                                    SizedBox(
                                    height: 25,
                                      ),
                                    Center(child: Text("No disease, You are healthy maccha !!")),
# DOCTOR-X

done using Flutter

In medical field one common problem faced by people is to deal with big list of medical tests
even when not needed which increases the cost of treatment. This is mainly because of
doctor’s inability of predict exact disease. Another problem is patient’s negligence towards
some simple symptoms which may potentially a serious health issue, but the refrain from
going to doctor fearing of spending thousands on medical tests and outcome being some
simple heath issue or none at all.

Our idea is to make the task of predicting a disease easier for doctor and give a virtual
doctor to every person with which he can share his symptoms and get to know probable
health issue and should he actually visit a doctor.

We will have a user interface which takes input as person’s age, gender, weight, physical
body symptoms and psychological symptoms. Using artificial neural network we train a
model which takes medical data like symptoms and age as features and diseases as output.
If probability of two disease is very close as computed by model then it will suggest a
medical test on one of the diseases to confirm. After the model performs satisfactorily on
training set we can go for real world implementations by adding more features to
application like :-

### Tech

virtual doctor uses a number of open source projects to work properly:
Flutter :To build a user interface an take input of symptoms from user
Neural Network : A machine learning approach to predict disease
Dataset : to train the model

### Installation
Doctor X has been programmed in flutter

install flutter
Install Android studio


### Development

# doctorx

A new Flutter application.

## Creating the frontend to take user input
    ##first we create a dropdown button to take in "body condition" type of symptoms

                            DropdownButton<String>(
                                    hint: Text("Body Conditions"),
                                           items: <String>[
                                             'Loose Motions',
                                             'Rashes',
                                             'Vomiting',
                                             'Loss of appetite',
                                             'Skin Wrinkling',
                                             'Dry mucus',
                                             'Coughing',
                                             'Too much Thirst',
                                             'Yello Eye',
                                             'Yellow Skin',
                                             'Yellow Urine',
                                             'Itching',
                                             'Weight Loss',
                                             'Pox',
'

            Similarly 3 more drop downs namely physical pains" "psychological conditions" and "fever range" is created

    ##then we create a floating ction button to add new dropdown field if user want to enter more symptoms
                             FloatingActionButton(onPressed: () {},child: Icon(Icons.add),)


    ##We also need a parameter to judge how confident a user is about his symptom which in terms give us probability of the the symptom to be present in the patient.
                (in bayesian learing approach this gives us prior probability of occurance of an event)

                                  Spacer(),StarRating(size: 25,rating: rating2,onRatingChanged: (rt){
                                          setState(() {
                                            rating2=rt;

    ##and finally a submittion button and a field to show final output
                             SizedBox(
                                     height: 20,
                                        ),
                                      Center(child: FloatingActionButton(child: Icon(Icons.done),)),
                                    SizedBox(
                                    height: 25,
                                      ),
                                    Center(child: Text("No disease, You are healthy maccha !!")),
