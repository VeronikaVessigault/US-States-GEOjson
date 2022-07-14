# US-States-GEOjson
# GEOjson to be used with Mapbox/Plotly.

# Comprehensive dictionary that takes the 50 states and connects it to the ID that Mapbox will use for graphing.

us_state_to_id = {'Alabama': '01', 'Alaska': '02', 'Arizona': '04', 'Arkansas': '05', 'California': '06', 'Colorado': '08',
                  'Connecticut': '09', 'Delaware': '10', 'Florida': '12', 'Georgia': '13', 'Hawaii': '15', 'Idaho': '16',
                  'Illinois': '17', 'Indiana': '18', 'Iowa': '19', 'Kansas': '20', 'Kentucky': '21', 'Louisiana': '22',
                  'Maine': '23', 'Maryland': '24', 'Massachusetts': '25', 'Michigan': '26', 'Minnesota': '27',
                  'Mississippi': '28', 'Missouri': '29', 'Montana': '30', 'Nebraska': '31', 'Nevada': '32',
                  'New Hampshire': '33', 'New Jersey': '34', 'New Mexico': '35', 'New York': '36', 'North Carolina': '37',
                  'North Dakota': '38', 'Ohio': '39', 'Oklahoma': '40', 'Oregon': '41', 'Pennsylvania': '42',
                  'Rhode Island': '44', 'South Carolina': '45', 'South Dakota': '46', 'Tennessee': '47', 'Texas': '48',
                  'Utah': '49', 'Vermont': '50', 'Virginia': '51', 'Washington': '53', 'West Virginia': '54',
                  'Wisconsin': '55', 'Wyoming': '56'}

# Other dictionaries, lists, and functions that may be useful for this GEOjson, all lists are alphebetically ordered by the full state name they correspond to.

US_ALL_STATES = ["Alabama","Alaska","Arizona","Arkansas","California","Colorado", "Connecticut","Delaware",
                 "Florida","Georgia","Hawaii","Idaho","Illinois","Indiana","Iowa","Kansas","Kentucky","Louisiana",
                 "Maine","Maryland","Massachusetts","Michigan","Minnesota","Mississippi","Missouri","Montana",
                 "Nebraska","Nevada","New Hampshire","New Jersey","New Mexico","New York","North Carolina",
                 "North Dakota","Ohio","Oklahoma","Oregon","Pennsylvania","Rhode Island","South Carolina",
                 "South Dakota","Tennessee","Texas","Utah","Vermont","Virginia","Washington","West Virginia",
                 "Wisconsin","Wyoming"]

US_ALL_STATES_ABBREVIATED = ['AL', 'AK', 'AZ', 'AR', 'CA', 'CO', 'CT', 'DE', 'FL', 'GA', 'HI', 'ID', 'IL', 'IN', 'IA',
                             'KS', 'KY', 'LA', 'ME', 'MD', 'MA', 'MI', 'MN', 'MS', 'MO', 'MT', 'NE', 'NV', 'NH', 'NJ',
                             'NM', 'NY', 'NC', 'ND', 'OH', 'OK', 'OR', 'PA', 'RI', 'SC', 'SD', 'TN', 'TX', 'UT', 'VT',
                             'VA', 'WA', 'WV', 'WI', 'WY']

us_state_to_abbrev = {"Alabama": "AL","Alaska": "AK","Arizona": "AZ","Arkansas": "AR","California": "CA",
                      "Colorado": "CO","Connecticut": "CT","Delaware": "DE","Florida": "FL","Georgia": "GA",
                      "Hawaii": "HI","Idaho": "ID","Illinois": "IL","Indiana": "IN","Iowa": "IA","Kansas": "KS",
                      "Kentucky": "KY","Louisiana": "LA","Maine": "ME","Maryland": "MD","Massachusetts": "MA",
                      "Michigan": "MI","Minnesota": "MN","Mississippi": "MS","Missouri": "MO","Montana": "MT",
                      "Nebraska": "NE","Nevada": "NV","New Hampshire": "NH","New Jersey": "NJ","New Mexico": "NM",
                      "New York": "NY","North Carolina": "NC","North Dakota": "ND","Ohio": "OH","Oklahoma": "OK",
                      "Oregon": "OR","Pennsylvania": "PA","Rhode Island": "RI","South Carolina": "SC","South Dakota": "SD",
                      "Tennessee": "TN","Texas": "TX","Utah": "UT","Vermont": "VT","Virginia": "VA","Washington": "WA",
                      "West Virginia": "WV","Wisconsin": "WI","Wyoming": "WY","District of Columbia": "DC",
                      "American Samoa": "AS","Guam": "GU","Northern Mariana Islands": "MP","Puerto Rico": "PR",
                      "United States Minor Outlying Islands": "UM","U.S. Virgin Islands": "VI"}

US_ALL_STATES_ID = ['01', '02', '04', '05', '06', '08', '09', '10', '12', '13', '15', '16', '17', '18', '19', '20',
                    '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36',
                    '37', '38', '39', '40', '41', '42', '44', '45', '46', '47', '48', '49', '50', '51', '53', '54',
                    '55', '56']

def US_State_Abbreviated(state):
    if (state in US_ALL_STATES):
        for i in range(0,51):
            if US_ALL_STATES[i] == state:
                return US_ALL_STATES_ABBREVIATED[i]

def US_State_ID(state):
    if (state in US_ALL_STATES):
        return us_state_to_id[state]
