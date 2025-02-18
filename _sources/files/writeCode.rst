Write Code Questions
--------------------
The following data file ``uspoll.txt`` is used in some of the questions in this section. The data
is ``City, State: PM10: PM2.5``.  PM 10 is annual mean amounts of particulate pollution that’s over 2.5 and less than 10
micrometers in diameter, and PM2.5 is the  annual mean amounts of particulate pollution
that’s 2.5 micrometers or less in diameter. Click show to see all of the data
and hide to put it away.

.. reveal:: pol_Data_8_10
    :showtitle: Show
    :hidetitle: Hide

    .. raw:: html

       <pre id="uspoll.txt">
       Aberdeen, SD :13 :8
       Adrian, MI :15 :9
       Akron, OH :18 :11
       Albany, GA :18 :11
       Albany-Lebanon, OR :14 :8
       Albany-Schenectady-Troy, NY :13 :8
       Albuquerque, NM :12 :7
       Alexandria, LA :20 :12
       Allegan, MI :14 :9
       Allentown-Bethlehem-Easton, PA-NJ :21 :12
       Altoona, PA :19 :12
       Anchorage, AK :13 :8
       Anderson, IN :18 :11
       Ann Arbor, MI :16 :10
       Appleton, WI :14 :9
       Asheville, NC :15 :9
       Athens, OH :14 :9
       Athens, TN :15 :9
       Athens-Clarke County, GA :16 :9
       Atlanta-Sandy Springs-Marietta, GA :23 :14
       Atlantic City-Hammonton, NJ :14 :8
       Augusta-Richmond County, GA-SC :18 :11
       Augusta-Waterville, ME :14 :9
       Austin-Round Rock, TX :17 :10
       Bakersfield, CA :24 :15
       Baltimore-Towson, MD :20 :12
       Bangor, ME :12 :7
       Baraboo, WI :17 :10
       Baton Rouge, LA :19 :11
       Bay City, MI :13 :8
       Beaver Dam, WI :15 :9
       Beckley, WV :14 :8
       Bellingham, WA :7 :4
       Bennington, VT :11 :7
       Birmingham-Hoover, AL :20 :12
       Bishop, CA :11 :6
       Bismarck, ND :11 :6
       Bloomington, IN :17 :10
       Bloomington-Normal, IL :16 :9
       Boise City-Nampa, ID :17 :10
       Boone, NC :13 :8
       Boston-Cambridge-Quincy, MA-NH :16 :10
       Boulder, CO :12 :7
       Bowling Green, KY :17 :10
       Bradenton-Sarasota-Venice, FL :12 :7
       Brainerd, MN :8 :5
       Bremerton-Silverdale, WA :7 :4
       Bridgeport-Stamford-Norwalk, CT :16 :9
       Brigham City, UT :12 :7
       Brookings, SD :14 :9
       Brownsville-Harlingen, TX :16 :10
       Brunswick, GA :13 :8
       Buffalo-Niagara Falls, NY :16 :9
       Burlington, NC :14 :9
       Burlington-South Burlington, VT :12 :7
       Butte-Silver Bow, MT :19 :11
       Cadillac, MI :10 :6
       Cambridge, MD :13 :8
       Canton-Massillon, OH :21 :12
       Cape Coral-Fort Myers, FL :12 :7
       Casper, WY :9 :5
       Cedar Rapids, IA :16 :10
       Champaign-Urbana, IL :16 :10
       Charleston, WV :18 :11
       Charleston-North Charleston-Summerville, SC :16 :10
       Charlotte-Gastonia-Concord, NC-SC :16 :10
       Charlottesville, VA :13 :8
       Chattanooga, TN-GA :18 :11
       Cheyenne, WY :9 :6
       Chicago-Naperville-Joliet, IL-IN-WI :22 :13
       Chico, CA :12 :7
       Cincinnati-Middletown, OH-KY-IN :23 :14
       Clarksburg, WV :16 :10
       Clarksville, TN-KY :16 :10
       Clearlake, CA :7 :4
       Cleveland-Elyria-Mentor, OH :24 :15
       Clinton, IA :18 :11
       Colorado Springs, CO :12 :7
       Columbia, SC :17 :10
       Columbia, TN :14 :8
       Columbus, GA-AL :19 :11
       Columbus, OH :18 :11
       Concord, NH :16 :9
       Cookeville, TN :14 :9
       Corning, NY :11 :7
       Corpus Christi, TX :18 :11
       Dallas-Fort Worth-Arlington, TX :20 :12
       Daphne-Fairhope-Foley, AL :15 :9
       Davenport-Moline-Rock Island, IA-IL :18 :11
       Dayton, OH :18 :11
       Decatur, AL :15 :9
       Decatur, IL :17 :10
       Deltona-Daytona Beach-Ormond Beach, FL :11 :6
       Denver-Aurora-Broomfield, CO :14 :9
       Des Moines-West Des Moines, IA :15 :9
       Detroit-Warren-Livonia, MI :21 :12
       Dickinson, ND :7 :4
       Dothan, AL :15 :9
       Dover, DE :14 :8
       Duluth, MN-WI :11 :6
       Durango, CO :7 :4
       Durham, NC :14 :8
       Durham-Chapel Hill, NC :14 :8
       Dyersburg, TN :15 :9
       East Stroudsburg, PA :13 :8
       Eau Claire, WI :14 :8
       El Centro, CA :24 :14
       El Dorado, AR :18 :11
       El Paso, TX :21 :12
       Elizabethtown, KY :20 :12
       Elkhart-Goshen, IN :21 :12
       Erie, PA :19 :11
       Eugene-Springfield, OR :13 :8
       Eureka-Arcata-Fortuna, CA :11 :7
       Evansville, IN-KY :19 :12
       Fairbanks, AK :31 :19
       Fairmont, WV :17 :10
       Fargo, ND-MN :13 :8
       Farmington, NM :8 :5
       Fayetteville, NC :15 :9
       Fayetteville-Springdale-Rogers, AR-MO :16 :10
       Flagstaff, AZ :9 :5
       Flint, MI :13 :8
       Florence, SC :15 :9
       Florence-Muscle Shoals, AL :15 :9
       Fort Collins-Loveland, CO :12 :7
       Fort Madison-Keokuk, IA-MO :18 :11
       Fort Payne, AL :15 :9
       Fort Smith, AR-OK :17 :10
       Fort Wayne, IN :23 :14
       Fresno, CA :74 :45
       Gadsden, AL :16 :10
       Gainesville, FL :12 :7
       Gainesville, GA :16 :9
       Gettysburg, PA :18 :11
       Gillette, WY :13 :8
       Goldsboro, NC :21 :13
       Grand Island, NE :13 :8
       Grand Junction, CO :12 :7
       Grand Rapids-Wyoming, MI :16 :10
       Grants Pass, OR :12 :7
       Greeley, CO :13 :8
       Green Bay, WI :16 :10
       Greensboro-High Point, NC :14 :9
       Greenville, NC :13 :8
       Greenville-Mauldin-Easley, SC :16 :10
       Grenada, MS :16 :9
       Gulfport-Biloxi, MS :16 :10
       Hagerstown-Martinsburg, MD-WV :19 :11
       Hammond, LA :15 :9
       Hanford-Corcoran, CA :28 :17
       Harriman, TN :22 :13
       Harrisburg-Carlisle, PA :20 :12
       Harrisonburg, VA :15 :9
       Hartford-West Hartford-East Hartford, CT :14 :9
       Hattiesburg, MS :18 :11
       Helena, MT :16 :9
       Helena-West Helena, AR :16 :9
       Hickory-Lenoir-Morganton, NC :16 :10
       Hilo, HI :27 :16
       Hobbs, NM :13 :8
       Holland-Grand Haven, MI :15 :9
       Homosassa Springs, FL :11 :7
       Honolulu, HI :12 :7
       Hot Springs, AR :18 :11
       Houma-Bayou Cane-Thibodaux, LA :13 :8
       Houston-Sugar Land-Baytown, TX :21 :13
       Huntington-Ashland, WV-KY-OH :19 :11
       Huntsville, AL :16 :9
       Indianapolis-Carmel, IN :25 :15
       Iowa City, IA :16 :10
       Jackson, MS :19 :11
       Jackson, TN :15 :9
       Jackson, WY-ID :11 :6
       Jacksonville, FL :13 :8
       Jamestown-Dunkirk-Fredonia, NY :13 :8
       Jasper, IN :18 :11
       Johnstown, PA :19 :12
       Juneau, AK :11 :6
       Kahului-Wailuku, HI :11 :6
       Kalamazoo-Portage, MI :17 :10
       Kalispell, MT :13 :8
       Kansas City, MO-KS :24 :15
       Kapaa, HI :11 :7
       Keene, NH :16 :10
       Kingsport-Bristol-Bristol, TN-VA :15 :9
       Kinston, NC :13 :8
       Klamath Falls, OR :18 :11
       Knoxville, TN :18 :11
       Kokomo, IN :16 :10
       La Crosse, WI-MN :14 :8
       Laconia, NH :11 :7
       Lafayette, IN :24 :14
       Lafayette, LA :18 :11
       Lake Charles, LA :14 :8
       Lake Havasu City-Kingman, AZ :6 :4
       Lakeland-Winter Haven, FL :13 :8
       Lancaster, PA :21 :13
       Lansing-East Lansing, MI :14 :9
       Laramie, WY :9 :6
       Las Cruces, NM :25 :15
       Las Vegas-Paradise, NV :20 :12
       Laurel, MS :18 :11
       Lawrenceburg, TN :14 :8
       Lebanon, NH-VT :11 :7
       Lebanon, PA :24 :14
       Lewiston-Auburn, ME :13 :8
       Lexington-Fayette, KY :16 :10
       Lima, OH :17 :10
       Lincoln, NE :14 :9
       Little Rock-North Little Rock-Conway, AR :19 :12
       Logan, UT-ID :15 :9
       Los Angeles-Long Beach-Santa Ana, CA :33 :20
       Louisville/Jefferson County, KY-IN :22 :13
       Lumberton, NC :14 :9
       Lynchburg, VA :13 :8
       Macon, GA :19 :12
       Madera, CA :27 :16
       Madison, WI :16 :9
       Manchester-Nashua, NH :14 :8
       Marshall, MN :12 :7
       Marshall, TX :17 :10
       McAlester, OK :19 :11
       McAllen-Edinburg-Mission, TX :18 :11
       Medford, OR :15 :9
       Memphis, TN-MS-AR :17 :10
       Merced, CA :18 :11
       Meridian, MS :17 :10
       Miami-Fort Lauderdale-Pompano Beach, FL :14 :8
       Michigan City-La Porte, IN :16 :10
       Middlesborough, KY :17 :10
       Milwaukee-Waukesha-West Allis, WI :18 :11
       Minneapolis-St. Paul-Bloomington, MN-WI :17 :10
       Missoula, MT :21 :12
       Mobile, AL :15 :9
       Modesto, CA :25 :15
       Monroe, LA :22 :13
       Monroe, MI :16 :9
       Montgomery, AL :18 :11
       Morgantown, WV :15 :9
       Mount Vernon, IL :14 :9
       Muncie, IN :16 :10
       Muscatine, IA :18 :11
       Muskegon-Norton Shores, MI :15 :9
       Napa, CA :23 :14
       Nashville-Davidson--Murfreesboro--Franklin, TN :17 :10
       New Castle, IN :15 :9
       New Haven-Milford, CT :15 :9
       New Orleans-Metairie-Kenner, LA :21 :13
       New York-Northern New Jersey-Long Island, NY-NJ-PA :23 :14
       Niles-Benton Harbor, MI :14 :9
       Nogales, AZ :16 :10
       Norwich-New London, CT :13 :8
       Ogden-Clearfield, UT :15 :9
       Oklahoma City, OK :16 :10
       Omaha-Council Bluffs, NE-IA :19 :12
       Orlando-Kissimmee, FL :12 :7
       Owensboro, KY :18 :11
       Oxnard-Thousand Oaks-Ventura, CA :16 :10
       Paducah, KY-IL :17 :10
       Palm Bay-Melbourne-Titusville, FL :10 :6
       Parkersburg-Marietta-Vienna, WV-OH :17 :10
       Pascagoula, MS :15 :9
       Pendleton-Hermiston, OR :12 :7
       Pensacola-Ferry Pass-Brent, FL :14 :8
       Peoria, IL :16 :10
       Philadelphia-Camden-Wilmington, PA-NJ-DE-MD :28 :17
       Phoenix-Mesa-Scottsdale, AZ :26 :16
       Pittsburgh, PA :25 :15
       Pittsfield, MA :14 :9
       Platteville, WI :15 :9
       Pocatello, ID :15 :9
       Ponca City, OK :17 :10
       Portland-South Portland-Biddeford, ME :15 :9
       Portland-Vancouver-Beaverton, OR-WA :12 :7
       Portsmouth, OH :16 :10
       Poughkeepsie-Newburgh-Middletown, NY :13 :8
       Prescott, AZ :7 :4
       Prineville, OR :14 :9
       Providence-New Bedford-Fall River, RI-MA :18 :11
       Provo-Orem, UT :14 :8
       Pueblo, CO :11 :7
       Quincy, IL-MO :16 :10
       Raleigh-Cary, NC :16 :9
       Rapid City, SD :11 :6
       Reading, PA :19 :11
       Red Bluff, CA :14 :8
       Redding, CA :10 :6
       Reno-Sparks, NV :15 :9
       Richmond, VA :15 :9
       Richmond-Berea, KY :15 :9
       Riverside-San Bernardino-Ontario, CA :34 :21
       Riverton, WY :13 :8
       Roanoke, VA :15 :9
       Rochester, MN :13 :8
       Rochester, NY :14 :9
       Rock Springs, WY :13 :8
       Rockford, IL :16 :9
       Rocky Mount, NC :13 :8
       Rome, GA :18 :11
       Russellville, AR :14 :9
       Rutland, VT :15 :9
       Sacramento--Arden-Arcade--Roseville, CA :15 :9
       Salinas, CA :10 :6
       Salisbury, NC :16 :9
       Salt Lake City, UT :15 :9
       San Antonio, TX :14 :9
       San Diego-Carlsbad-San Marcos, CA :24 :14
       San Francisco-Oakland-Fremont, CA :16 :10
       San Jose-Sunnyvale-Santa Clara, CA :16 :10
       San Luis Obispo-Paso Robles, CA :16 :10
       Santa Barbara-Santa Maria-Goleta, CA :14 :9
       Santa Cruz-Watsonville, CA :10 :6
       Santa Fe, NM :8 :5
       Santa Rosa-Petaluma, CA :14 :8
       Sault Ste. Marie, MI :14 :8
       Savannah, GA :17 :10
       Scottsbluff, NE :9 :6
       Scranton--Wilkes-Barre, PA :14 :8
       Seaford, DE :14 :8
       Seattle-Tacoma-Bellevue, WA :16 :10
       Sheridan, WY :14 :8
       Shreveport-Bossier City, LA :26 :16
       Sierra Vista-Douglas, AZ :11 :7
       Sioux City, IA-NE-SD :16 :10
       Sioux Falls, SD :14 :9
       Somerset, KY :16 :10
       South Bend-Mishawaka, IN-MI :21 :13
       Spartanburg, SC :16 :10
       Spokane, WA :12 :7
       Springfield, IL :16 :10
       Springfield, MA :15 :9
       Springfield, MO :17 :10
       Springfield, OH :17 :10
       St. Cloud, MN :14 :8
       St. George, UT :11 :7
       St. Joseph, MO-KS :20 :12
       St. Louis, MO-IL :22 :13
       State College, PA :19 :11
       Stockton, CA :21 :12
       Syracuse, NY :12 :7
       Talladega-Sylacauga, AL :17 :10
       Tallahassee, FL :14 :9
       Tampa-St. Petersburg-Clearwater, FL :13 :8
       Terre Haute, IN :19 :12
       Texarkana, TX-Texarkana, AR :18 :11
       Thomasville-Lexington, NC :17 :10
       Toledo, OH :17 :10
       Topeka, KS :14 :9
       Torrington, CT :9 :6
       Trenton-Ewing, NJ :15 :9
       Truckee-Grass Valley, CA :10 :6
       Tucson, AZ :10 :6
       Tulsa, OK :16 :10
       Tupelo, MS :16 :10
       Tuscaloosa, AL :16 :9
       Ukiah, CA :12 :7
       Valdosta, GA :14 :9
       Vallejo-Fairfield, CA :15 :9
       Vernal, UT :12 :7
       Virginia Beach-Norfolk-Newport News, VA-NC :14 :8
       Visalia-Porterville, CA :25 :15
       Warner Robins, GA :16 :10
       Washington-Arlington-Alexandria, DC-VA-MD-WV :19 :12
       Waterloo-Cedar Falls, IA :16 :10
       Watertown, SD :18 :11
       Weirton-Steubenville, WV-OH :20 :12
       Wenatchee, WA :17 :10
       Wichita, KS :16 :9
       Wilmington, NC :14 :9
       Winchester, VA-WV :16 :10
       Winston-Salem, NC :15 :9
       Worcester, MA :15 :9
       Yakima, WA :17 :10
       York-Hanover, PA :20 :12
       Youngstown-Warren-Boardman, OH-PA :23 :14
       Yuba City, CA :12 :7
       Yuma, AZ :14 :9
       </pre>

.. datafile:: uspoll.txt
    :fromfile: uspoll.txt
    :hide:

#.
    .. tabbed:: file_ex_pollError

        .. tab:: Question

            Fix errors in the code below so that the code runs correctly and prints
            the pollution for all cities that start with the letter A.

            .. activecode:: file_ex_pollErrorq
                :datafile: uspoll.txt

                inFile = open("uspoll.txt","r)

                for line in inFile
                    values = line.split(":")
                    city = values[0]
                    if (city.find("A") == 0):
                        print('City: ' city)
                        print("Pollution values:",values[1],values[2])

                inFile.close()

        .. tab:: Answer

            It was missing a close double quote after the r on line 1.  It was missing a colon
            at the end of line 3.  It was missing a comma or plus sign between the values on line 7.

            .. activecode:: file_ex_pollErrora
                :optional:
                :datafile: uspoll.txt

                # Close quotations around "r"
                inFile = open("uspoll.txt","r")

                # Add a colon at the end
                for line in inFile:
                    values = line.split(":")
                    city = values[0]
                    if (city.find("A") == 0):
                        # "+" is needed to concatenate strings and variables
                        print('City: ' + city)
                        print("Pollution values:",values[1],values[2])

                inFile.close()

#.
    .. activecode::  file_ex_pmErrorq
        :datafile: uspoll.txt

        Fix the errors in the code below so that it returns the average PM 2.5 value
        for the passed state (using the two letter abbreviation).  Each line of the file is in the format ``City, State: PM10: PM2.5``. For example, the first line is "Aberdeen, SD :13 :8". It should
        print 11.33333333333333.
        ~~~~
        def avg_PM25(state)

            # get the lines from the file
            inFile = open("uspoll.txt","r")
            lines = inFile.readlines()
            inFile.close()

            # calculate the average
            total = 0
            count = 0
            for line in lines:
                values = line.split(":")
                curr25 = float(values[2])
                cityState = values[1]
                values = cityState.split(",")
                curr_state = values[0]
                if curr_state.find(state) >= 0:
                    total += curr25
                    count += 1

                return total / count

        print(avg_PM25('OH'))

#.
    .. tabbed:: file_ex_AorB

        .. tab:: Question

            The code below prints all the lines that have a city that starts with an "A".
            Change it so that it prints out all lines that have a city that starts with "A" or "B".

            .. activecode::  file_ex_AorBq
                :datafile: uspoll.txt

                inFile = open("uspoll.txt","r")
                lines = inFile.readlines()
                inFile.close()

                for line in lines:
                    if line[0] == "A":
                        print(line)
        .. tab:: Answer

            .. activecode:: file_ex_AorBa
                :datafile: uspoll.txt
                :optional:

                # Read all the lines
                inFile = open("uspoll.txt","r")
                lines = inFile.readlines()
                inFile.close()

                # Loop through the lines
                for line in lines:
                    # Set condition for lines starting with A or B
                    # Be sure to close parentheses to separate phrases
                    if (line[0] == "A") | (line[0] == "B"):
                        print(line)


#.
    .. activecode:: file_ex_valueCity
        :datafile: uspoll.txt

        Fix the indention below for the code to correctly find and print the lowest 2.5 value and city.
        It should print ``Smallest PM 2.5  4.0  in  Bellingham, WA``.
        ~~~~
        inFile = open("uspoll.txt","r")
        lines = inFile.readlines()
        inFile.close()

        minCity = ''
        min25 = 500
        for line in lines:
        values = line.split(":")
        new25 = float(values[2])
        if new25 < min25:
        minCity = values[0]
        min25 = new25
        print("Smallest PM 2.5 ",min25," in ",minCity)

#.
    .. tabbed:: file_ex_test

        .. tab:: Question

            The following sample file called ``studentdata.txt`` contains one line for each student
            in an imaginary class. The students name is the first thing on each line, followed by
            some exam scores. The number of scores might be different for each student.

            .. raw:: html

                <pre id="studentdata.txt">
                joe 10 15 20 30 40
                bill 23 16 19 22
                sue 8 22 17 14 32 17 24 21 2 9 11 17
                grace 12 28 21 45 26 10
                john 14 32 25 16 89
                </pre>

            Using the text file ``studentdata.txt`` write a program that prints out the names of
            students that have six or more quiz scores.

            .. activecode:: file_ex_testq
                :available_files: studentdata.txt

                # Hint: first see if you can write a program that just prints out the number of scores on each line
                # Then, make it print the number only if the number is at least six
                # Then, switch it to printing the name instead of the number



        .. tab:: Answer

            .. activecode:: file_ex_testa
                :optional:

                # Open the file in "read" mode
                f = open("studentdata.txt", "r")

                # iterate through lines in the file
                for aline in f:
                    # Split each item of the line
                    items = aline.split()
                    # Set condition for student that have 6 or more quiz scores
                    # Element 0 is the name, so start with element 1
                    if len(items[1:]) >= 6:
                        # Print the name (element 0) if the condition is met
                        print(items[0])
                # Close the file
                f.close()

The following file contains a set of emotions that will be used in the next question.



.. raw:: html

    <pre id="emotion_words.txt">
    Sad upset blue down melancholy somber bitter troubled
    Angry mad enraged irate irritable wrathful outraged infuriated
    Happy cheerful content elated joyous delighted lively glad
    Confused disoriented puzzled perplexed dazed befuddled
    Excited eager thrilled delighted
    Scared afraid fearful panicked terrified petrified startled
    Nervous anxious jittery jumpy tense uneasy apprehensive
    </pre>

#.
    .. activecode:: file_ex_emotionq
       :available_files: emotion_words.txt

       Create a list called ``j_emotions`` that contains every word in ``emotion_words.txt``
       that begins with the letter "j".  After the code executes ``j_emotions`` should be ``['joyous', 'jittery', 'jumpy']``
       ~~~~


       =====

       from unittest.gui import TestCaseGui

       class myTests(TestCaseGui):

          def testOne(self):
             self.assertEqual(j_emotions, ['joyous', 'jittery', 'jumpy'], "Testing that j_emotions was created correctly.")

       myTests().main()

The rest of the questions gather their data from the file ``stocks.txt``, which shows the monthly Dow
Jones averages from 1989 to 2001. The data is in the order: Date, Open, High, Low, Close, Volume. The first
line is ``3-Dec-01,9848.93,10220.78,9651.87,10021.57``.  The Date is in the format ``d-Month-yy``.  The month
is the first three letters of the month.

.. reveal:: pol_Data_8_10_2
   :showtitle: Show
   :hidetitle: Hide

   .. raw:: html

      <pre id="stocks.txt">
      3-Dec-01,9848.93,10220.78,9651.87,10021.57
      1-Nov-01,9087.45,10054.58,8987.61,9851.56
      1-Oct-01,8845.97,9626.54,8659.9,9075.14
      4-Sep-01,9946.98,10238.5,7926.93,8847.56
      1-Aug-01,10527.38,10663.07,9829.35,9949.75
      2-Jul-01,10504.95,10758.14,10049.38,10522.81
      1-Jun-01,10913.57,11236.68,10313.4,10502.4
      1-May-01,10734.05,11436.42,10638.48,10911.94
      2-Apr-01,9877.16,10973.15,9303.48,10734.97
      1-Mar-01,10493.25,10940.45,9047.56,9878.78
      1-Feb-01,10884.82,11140.09,10225.14,10495.28
      2-Jan-01,10790.92,11224.41,10325.71,10887.36
      1-Dec-00,10416.76,11044.7,10158.16,10787.99
      1-Nov-00,10966.21,11152.02,10204.8,10414.49
      2-Oct-00,10659.06,11108.79,9571.4,10971.14
      1-Sep-00,11219.54,11518.83,10439.31,10650.92
      1-Aug-00,10523.81,11415.99,10428.58,11215.1
      3-Jul-00,10450.36,10980.34,10303.28,10521.98
      1-Jun-00,10532.27,11013.05,10161.51,10447.89
      1-May-00,10749.42,11086.72,10163.2,10522.33
      3-Apr-00,10863.28,11600.43,10128.62,10733.91
      1-Mar-00,10128.11,11311.28,9611.75,10921.92
      1-Feb-00,10937.74,11228.44,9760.36,10128.31
      3-Jan-00,11501.85,11908.5,10610.43,10940.53
      1-Dec-99,10876.47,11658.68,10798.07,11497.12
      1-Nov-99,10730.78,11195.34,10449.42,10877.81
      1-Oct-99,10335.69,10883.1,9884.2,10729.86
      1-Sep-99,10828.44,11218.39,10055.17,10336.95
      2-Aug-99,10654.83,11428.94,10487.34,10829.28
      1-Jul-99,10972.39,11321.61,10594.99,10655.15
      1-Jun-99,10549.08,11120.24,10334.42,10970.8
      3-May-99,10788.75,11244.36,10372.96,10559.74
      1-Apr-99,9825.29,11072.25,9707.91,10789.04
      1-Mar-99,9315.27,10158.57,9163.41,9786.16
      1-Feb-99,9405.43,9662.77,9025.41,9306.58
      4-Jan-99,9212.84,9759.44,8994.26,9358.83
      1-Dec-98,9039.57,9390.75,8610.63,9181.43
      2-Nov-98,8645.65,9457.95,8573.56,9116.55
      1-Oct-98,7749.42,8718.25,7399.78,8592.1
      1-Sep-98,7583.09,8253.79,7379.7,7842.62
      3-Aug-98,8868.1,8948.17,7517.7,7539.07
      1-Jul-98,9011.56,9412.64,8786.48,8883.29
      1-Jun-98,8907.93,9155.04,8524.55,8952.02
      1-May-98,9106.47,9311.98,8760.95,8899.95
      1-Apr-98,8818.5,9287.32,8715.61,9063.37
      2-Mar-98,8528.78,8997.11,8377.32,8799.81
      2-Feb-98,7987.46,8616.72,7987.46,8545.72
      2-Jan-98,7908.25,8072.91,7391.59,7906.5
      1-Dec-97,7823.62,8209.56,7563.23,7908.25
      3-Nov-97,7443.07,7934.53,7334.77,7823.13
      1-Oct-97,7945.26,8218.34,6936.45,7442.08
      2-Sep-97,7650.99,8078.36,7556.23,7945.26
      1-Aug-97,8222.61,8340.14,7580.85,7622.42
      1-Jul-97,7672.79,8328.99,7613.53,8222.61
      2-Jun-97,7331.04,7868.44,7214.29,7672.79
      1-May-97,7008.99,7430.2,6891.39,7331.04
      1-Apr-97,6583.48,7081.23,6315.84,7008.99
      3-Mar-97,6877.74,7158.28,6532.49,6583.48
      3-Feb-97,6813.09,7112.87,6683.4,6877.74
      2-Jan-97,6448.27,6953.55,6318.96,6813.09
      2-Dec-96,6521.7,6623.96,6206.83,6448.27
      1-Nov-96,6029.38,6606.3,5975.34,6521.7
      1-Oct-96,5882.17,6162.8,5833.72,6029.38
      3-Sep-96,5616.21,5952.08,5550.37,5882.17
      1-Aug-96,5528.91,5761.95,5507.83,5616.21
      1-Jul-96,5654.63,5769.88,5170.11,5528.91
      3-Jun-96,5643.18,5770.61,5559.69,5654.63
      1-May-96,5569.08,5833.04,5327.74,5643.18
      1-Apr-96,5587.14,5737.07,5382.66,5569.08
      1-Mar-96,5485.62,5755.86,5395.3,5587.14
      1-Feb-96,5395.3,5693.36,5319.43,5485.62
      2-Jan-96,5117.12,5433.24,5000.07,5395.3
      1-Dec-95,5074.49,5266.69,5016.68,5117.12
      1-Nov-95,4755.48,5143.13,4719.72,5074.49
      2-Oct-95,4789.08,4845.08,4638.43,4755.48
      1-Sep-95,4610.56,4839.48,4594.71,4789.08
      1-Aug-95,4708.47,4772.56,4552.8,4610.56
      3-Jul-95,4556.1,4767.99,4530.26,4708.47
      1-Jun-95,4465.14,4614.2,4394.59,4556.1
      1-May-95,4321.27,4480.7,4278.73,4465.14
      3-Apr-95,4157.69,4348.94,4129.68,4321.27
      1-Mar-95,4011.05,4213.71,3935.31,4157.69
      1-Feb-95,3843.86,4034.62,3809.21,4011.05
      3-Jan-95,3834.44,3955.56,3794.4,3843.86
      1-Dec-94,3739.23,3882.21,3638.97,3834.44
      1-Nov-94,3908.12,3919.9,3612.05,3739.23
      3-Oct-94,3843.19,3958.25,3736.2,3908.12
      1-Sep-94,3913.42,3972.72,3804.5,3843.19
      1-Aug-94,3764.5,3954.54,3722.41,3913.42
      1-Jul-94,3624.96,3782.63,3611.04,3764.5
      1-Jun-94,3758.37,3839.88,3603.92,3624.96
      2-May-94,3681.69,3788.76,3609.71,3758.37
      4-Apr-94,3633.08,3733.15,3520.8,3681.69
      1-Mar-94,3832.02,3911.78,3544.12,3635.96
      1-Feb-94,3978.36,3998.06,3811.76,3832.02
      3-Jan-94,3754.09,4002.84,3715.24,3978.36
      1-Dec-93,3683.95,3818.92,3673.33,3754.09
      1-Nov-93,3680.59,3749.9,3585.86,3683.95
      1-Oct-93,3555.12,3713.57,3541.71,3680.59
      1-Sep-93,3651.25,3665.5,3501.47,3555.12
      2-Aug-93,3539.47,3681.71,3523.54,3651.25
      1-Jul-93,3516.08,3604.86,3443.28,3539.47
      1-Jun-93,3527.43,3577.25,3445.77,3516.08
      3-May-93,3427.55,3582.23,3402.42,3527.43
      1-Apr-93,3435.11,3499.41,3338.39,3427.55
      1-Mar-93,3370.81,3497.25,3334.07,3435.11
      1-Feb-93,3310.03,3472.94,3262.48,3370.81
      4-Jan-93,3301.11,3338.12,3219.25,3310.03
      1-Dec-92,3305.16,3364.87,3229.79,3301.11
      2-Nov-92,3226.28,3326.51,3176.84,3305.16
      1-Oct-92,3271.66,3291.39,3087.41,3226.28
      1-Sep-92,3257.35,3391.35,3226.55,3271.66
      3-Aug-92,3393.78,3413.23,3200.86,3257.35
      1-Jul-92,3318.52,3414.85,3255.43,3393.78
      1-Jun-92,3396.88,3435.27,3242.32,3318.52
      1-May-92,3359.12,3433.98,3316.64,3396.88
      1-Apr-92,3235.47,3387.97,3141.77,3359.12
      2-Mar-92,3267.67,3318.42,3176.21,3235.47
      3-Feb-92,3223.39,3307.47,3193.42,3267.67
      2-Jan-92,3168.83,3313.51,3119.86,3223.39
      2-Dec-91,2894.68,3204.61,2832.29,3168.83
      1-Nov-91,3069.1,3091.91,2861.14,2894.68
      1-Oct-91,3016.77,3091.01,2925.54,3069.1
      3-Sep-91,3043.6,3066.64,2963.1,3016.77
      1-Aug-91,3024.82,3068.65,2836.31,3043.6
      1-Jul-91,2911.67,3039.58,2897.36,3024.82
      3-Jun-91,3027.5,3057.47,2879.25,2906.75
      1-May-91,2887.87,3044.5,2834.53,3027.5
      1-Apr-91,2913.86,3030.45,2848.51,2887.87
      1-Mar-91,2882.18,3017.82,2829.21,2913.86
      1-Feb-91,2736.39,2955.2,2694.31,2882.18
      2-Jan-91,2633.66,2747.28,2447.03,2736.39
      3-Dec-90,2559.65,2662.62,2534.65,2633.66
      1-Nov-90,2442.33,2581.19,2415.59,2559.65
      1-Oct-90,2452.48,2565.35,2344.31,2442.33
      4-Sep-90,2614.36,2665.35,2367.82,2452.48
      1-Aug-90,2905.2,2931.19,2459.41,2614.36
      2-Jul-90,2880.69,3024.26,2833.17,2905.2
      1-Jun-90,2876.66,2956.93,2821.53,2880.69
      1-May-90,2656.76,2908.21,2651.35,2876.66
      2-Apr-90,2707.21,2793.47,2627.7,2656.76
      1-Mar-90,2627.25,2775,2607.88,2707.21
      1-Feb-90,2590.54,2674.32,2540.99,2627.25
      2-Jan-90,2753.2,2834.04,2513.06,2590.54
      1-Dec-89,2706.27,2784.77,2658.7,2753.2
      1-Nov-89,2645.08,2718.22,2563.11,2706.27
      2-Oct-89,2692.82,2809.08,2496.93,2645.08
      1-Sep-89,2737.27,2768.24,2636.78,2692.82
      1-Aug-89,2660.66,2758.73,2619.71,2737.27
      3-Jul-89,2440.06,2668.25,2431.53,2660.66
      1-Jun-89,2480.15,2544.95,2412.94,2440.06
      1-May-89,2418.8,2521.63,2356.3,2480.15
      3-Apr-89,2293.62,2433.1,2282.07,2418.8
      1-Mar-89,2258.39,2351.07,2234.46,2293.62
      1-Feb-89,2342.32,2369.29,2232.14,2258.39
      3-Jan-89,2168.39,2350.18,2127.14,2342.32
      </pre>

.. datafile:: stocks.txt
    :fromfile: stocks.txt
    :hide:

#.
    .. tabbed:: file_ex_biggestLoss

      .. tab:: Question

          Complete the code at the ``#`` so that it prints out the date with the biggest
          loss from open to close.  Each line has: Date, Open, High, Low, Close, Volume
          It should print ``3-Aug-98 loss 1329.030000000001``.

          .. activecode::  file_ex_biggestLossq
              :datafile: stocks.txt

              def biggestLoss(file):
                  maxLoss = 0
                  lines = file.readlines()
                  for line in #:
                      values = line.split(",")
                      opening = float(values[#])
                      closing = float(values[4])
                      dailyLoss = opening # closing
                      if (dailyLoss # maxLoss):
                          maxLoss = dailyLoss
                          date = values[#]
                  print(date + " loss " + str(maxLoss))

              file = open("stocks.txt", "r")
              biggestLoss(file)

      .. tab:: Answer

          .. activecode:: file_ex_biggestLossA
              :datafile: stocks.txt
              :optional:

              def biggestLoss(file):
                  maxLoss = 0
                  lines = file.readlines()
                  # Use line to iterate through lines
                  for line in lines:
                      values = line.split(",")
                      # Element 1 in values accesses the opening values
                      opening = float(values[1])
                      closing = float(values[4])
                      # dailyLoss is the difference between opening and closing
                      dailyLoss = opening - closing
                      # Set condition if the dailyLoss is greater than the overall highest loss
                      if (dailyLoss > maxLoss):
                          maxLoss = dailyLoss
                          # Element 0 is the date
                          date = values[0]
                  print(date + " loss " + str(maxLoss))

              file = open("stocks.txt", "r")
              biggestLoss(file)

#.
    .. activecode:: file_ex_300
        :datafile: stocks.txt

        Fix the errors below so that the ``pointGain`` function returns a list of all the dates where the Dow
        Jones gained more than 300 points from open to close.  Each line has: Date, Open, High, Low, Close.
        There should be 22 dates.
        ~~~~
        def pointGain():
            file = open("stocks.txt", "r")
            date_list = []
            for lines in file:
            values = line.split()
            opening = str(values[2])
            closing = float(values[4])
            if (closing - opening) < 300:
                date_list.append(values[0])
            file.close()
            return date_list

        # read the data
        pointGain()

        from unittest.gui import TestCaseGui

        class myTests(TestCaseGui):

            def testOne(self):
                res = pointGain()
                self.assertEqual(len(res),22,"Length(list) == 22")
                self.assertEqual(res[0],"1-Nov-01")
                self.assertEqual(res[1],"2-Apr-01")

        myTests().main()

#.
    .. tabbed:: file_ex_June

        .. tab:: Question

            The code below prints all the dates and high price for dates that occur
            on the first day of the month (i.e. January 1, February 1...).
            Each line has: Date, Open, High, Low, Close, Volume Change it
            so that it prints the date and low price for all the dates that occur in June.

            .. activecode::  file_ex_Juneq
                :datafile: stocks.txt

                file = open("stocks.txt", "r")
                lines = file.readlines()
                for line in lines:
                    values = line.split(",")
                    date = values[0]
                    if date[0] == "1":
                        print(date + " had a high value of " + values[2])

        .. tab:: Answer

            .. activecode:: file_ex_Junea
                :datafile: stocks.txt
                :optional:

                file = open("stocks.txt", "r")
                lines = file.readlines()
                for line in lines:
                    values = line.split(",")
                    date = values[0]
                    # date[2:5] accesses the 3 characters that express the month
                    # if these are the letters for June, print the statement
                    if date[2:5] == "Jun":
                        print(date + " had a low value of " + values[3])


#.
    .. activecode:: file_ex_abbrq
        :practice: T
        :datafile: stocks.txt

        Write a function ``avg_month_close(lines, month)`` that takes the ``lines``
        from the stocks file in a list and the abbreviation for a ``month``
        (i.e. "Jan", "Feb") as parameters and returns the average value of the closing
        prices during that month for all the years in the file.
        Each line has: Date, Open, High, Low, Close, Volume

        ~~~~


        =====

        from unittest.gui import TestCaseGui

        class myTests(TestCaseGui):
            def setUp(self):
                file = open("stocks.txt", "r")
                self.lines = file.readlines()
                file.close()

            def testOne(self):
                self.assertEqual(int(avg_month_close(self.lines,"Jan")), 5640, "Testing Jan = 5640")
                self.assertEqual(int(avg_month_close(self.lines,"Feb")), 5622, "Testing Feb = 5622=")
                self.assertEqual(int(avg_month_close(self.lines,"Jun")), 5957, "Testing Jun = 5957")
                self.assertEqual(int(avg_month_close(self.lines,"Sep")), 5778, "Testing Jun = 5778")
                self.assertEqual(int(avg_month_close(self.lines,"Nov")), 6043, "Testing Jun = 6043")

        myTests().main()
