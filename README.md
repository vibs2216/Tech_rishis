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
