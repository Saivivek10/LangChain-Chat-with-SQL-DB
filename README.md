# LangChain: Chat with SQL Database 🦜

This project demonstrates how to use [LangChain](https://github.com/hwchase17/langchain) to build a chatbot that interacts with an SQL database. The application supports both SQLite and MySQL databases and uses the `ChatGroq` model for natural language processing.

## Features
- Chat with an SQLite or MySQL database.
- Use natural language queries to interact with your database.
- Clear message history functionality.
- Streamlit-based user interface for easy interaction.

## Prerequisites
- Python 3.8 or higher
- A valid Groq API key
- SQLite database file (`student.db`) or MySQL database credentials

## Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd Chat-SQL
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Place your SQLite database file (`student.db`) in the project directory, or ensure you have access to your MySQL database.

## Usage
1. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

2. Open the app in your browser (usually at `http://localhost:8501`).

3. Select the database type:
   - **SQLite**: The app will use the `student.db` file in the project directory.
   - **MySQL**: Provide your MySQL host, user, password, and database name in the sidebar.

4. Enter your Groq API key in the sidebar.

5. Start chatting with your database by entering natural language queries.

## File Structure
- `app.py`: Main application file.
- `student.db`: SQLite database file (not included, add your own).
- `requirements.txt`: Python dependencies.

## Example Queries
- "Show all students in the database."
- "What is the average grade of students?"
- "List all students who scored above 90."

## Notes
- The app uses the `StreamlitCallbackHandler` for real-time response streaming.
- The `ChatGroq` model is configured with the `llama-3.1-8b-instant` model.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- [LangChain](https://github.com/hwchase17/langchain)
- [Streamlit](https://streamlit.io/)
- [SQLAlchemy](https://www.sqlalchemy.org/)
