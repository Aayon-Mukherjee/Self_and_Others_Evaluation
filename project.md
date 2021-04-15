        from googleapiclient.discovery import build
        from google.oauth2 import service_account

        SERVICE_ACCOUNT_FILE = 'keys.json'
        SCOPES = ['https://www.googleapis.com/auth/spreadsheet/']

        creds =None
        creds = service_account.credentials.from_service_account_file(
                SERVICE_ACCOUNT_FILE, scopes=SCOPES)


        # The ID and range of a sample spreadsheet.
        SAMPLE_SPREADSHEET_ID = '1HfmpUI3zo7W3i_ipaRXQ1VQN8SfjfTX1fhow03rY-_Y'


        service = build('sheets', 'v4', credentials=creds)

        # Call the Sheets API
        sheet = service.spreadsheets()
        result = sheet.values().get(spreadsheetId=SAMPLE_SPREADSHEET_ID,
                                    range="Skills Chart!$A$2:$K$24").execute()
        values = result.get('values', [])
        print(values)

![Error](https://user-images.githubusercontent.com/55484239/114898732-0128c500-9e30-11eb-8242-9c52c874f6cc.JPG)
