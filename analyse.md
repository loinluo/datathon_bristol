# Datathon 2023

## Schedule

16:00 Test set released

18:00 Submission deadline

# Road accidents

* casualty_severity
* Visualization
* Input: Features of casulty/vehicle
* Output: Casualty severity (0: slight  1: fatal/serious)
* Metrics:

  * f1_score
  * roc

### Data Analyse

#### Casualty

 0   accident_reference                  64759 non-null  object
 1   vehicle_reference                   64759 non-null  int64
 2   casualty_reference                  64759 non-null  int64
 3   casualty_class                      64759 non-null  int64
 4   sex_of_casualty                     64759 non-null  int64
 5   age_of_casualty                     64759 non-null  int64
 6   age_band_of_casualty                64759 non-null  int64
 7   casualty_severity                   64759 non-null  int64
 8   pedestrian_location                 64759 non-null  int64
 9   pedestrian_movement                 64759 non-null  int64
 10  car_passenger                       64759 non-null  int64
 11  bus_or_coach_passenger              64759 non-null  int64
 12  pedestrian_road_maintenance_worker  64759 non-null  int64
 13  casualty_type                       64759 non-null  int64
 14  casualty_home_area_type             64759 non-null  int64
 15  casualty_imd_decile                 64759 non-null  int64
 16  lsoa_of_casualty                    64759 non-null  object

#### Vehicle

 0   accident_reference                94659 non-null  object
 1   vehicle_reference                 94659 non-null  int64
 2   vehicle_type                      94659 non-null  int64
 3   towing_and_articulation           94659 non-null  int64
 4   vehicle_manoeuvre                 94659 non-null  int64
 5   vehicle_direction_from            94659 non-null  int64
 6   vehicle_direction_to              94659 non-null  int64
 7   vehicle_location_restricted_lane  94659 non-null  int64
 8   junction_location                 94659 non-null  int64
 9   skidding_and_overturning          94659 non-null  int64
 10  hit_object_in_carriageway         94659 non-null  int64
 11  vehicle_leaving_carriageway       94659 non-null  int64
 12  hit_object_off_carriageway        94659 non-null  int64
 13  first_point_of_impact             94659 non-null  int64
 14  vehicle_left_hand_drive           94659 non-null  int64
 15  journey_purpose_of_driver         94659 non-null  int64
 16  sex_of_driver                     94659 non-null  int64
 17  age_of_driver                     94659 non-null  int64
 18  age_band_of_driver                94659 non-null  int64
 19  engine_capacity_cc                94659 non-null  int64
 20  propulsion_code                   94659 non-null  int64
 21  age_of_vehicle                    94659 non-null  int64
 22  generic_make_model                94659 non-null  object
 23  driver_imd_decile                 94659 non-null  int64
 24  driver_home_area_type             94659 non-null  int64
 25  lsoa_of_driver                    94659 non-null  object

* Number of vehicle is more than casualty
* For each casulty, we can find the corresponding vehicle by searching the vehicel with the same accident reference and vehicle reference
