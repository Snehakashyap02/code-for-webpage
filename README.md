<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Assessment Recommendation Tool</title>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css">
    <style>
        body {
            font-family: 'Verdana', sans-serif;
            background: linear-gradient(to right, #2c2c2c, #1a1a1a);
            color: #f5f5f5;
        }
        .navbar {
            background-color: #333;
        }
        .navbar-brand, .nav-link {
            color: #f5f5f5 !important;
        }
        .container {
            margin-top: 30px;
            border-radius: 15px;
            padding: 20px;
            background-color: #444;
        }
        .form-control {
            border-radius: 25px;
            background-color: #555;
            color: #f5f5f5;
            border: 1px solid #666;
        }
        .btn-primary {
            background-color: #007bff;
            border: none;
            border-radius: 25px;
            font-size: 0.7rem;
            padding: 3px 10px;
        }
        .btn-primary:hover {
            background-color: #0056b3;
        }
        .card {
            background-color: #444;
            color: #f5f5f5;
            border: none;
            border-radius: 20px;
        }
        .btn-secondary {
            background-color: #007bff;
            border: none;
            border-radius: 25px;
            font-size: 0.7rem;
        }
        .form-group {
            margin-bottom: 20px;
        }
        h2 {
            margin-bottom: 30px;
        }
    </style>
</head>
<body>
    <nav class="navbar navbar-expand-lg">
        <a class="navbar-brand" href="#">Assessment Tool</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarContent" aria-controls="navbarContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarContent"></div>
            <ul class="navbar-nav mr-auto">
                <li class="nav-item active">
                    <a class="nav-link" href="#">Home</a>
                </li>
            </ul>
        </div>
    </nav>
    <div class="container">
        <h2 class="text-center">Assessment Catalogue</h2>
        <form>
            <div class="form-group">
                <label for="jobTitle">Job Title:</label>
                <input type="text" class="form-control" id="jobTitle" placeholder="Enter job title">
            </div>
            <div class="form-group">
                <label for="industry">Industry:</label>
                <select class="form-control" id="industry">
                    <option value="">Select industry</option>
                    <option value="finance">Finance</option>
                    <option value="healthcare">Healthcare</option>
                    <option value="technology">Technology</option>
                    <option value="manufacturing">Manufacturing</option>
                    <option value="education">Education</option>
                </select>
            </div>
            <div class="form-group">
                <label for="skills">Required Skills:</label>
                <input type="text" class="form-control" id="skills" placeholder="Enter required skills (e.g., teamwork, problem-solving)">
            </div>
            <button type="button" class="btn btn-primary btn-block" onclick="fetchRecommendations()">Get Recommendations</button>
        </form>
        <div class="row mt-4" id="assessments-container"></div>
        <!-- Cards will be dynamically added here -->
    </div>
    <!-- Modal -->
    <div class="modal fade" id="assessmentModal" tabindex="-1" role="dialog" aria-labelledby="assessmentModalLabel" aria-hidden="true">
        <div class="modal-dialog" role="document">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="assessmentModalLabel">Assessment Details</h5>
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">&times;</span>
                    </button>
                </div>
                <div class="modal-body" id="assessment-modal-body">
                    <!-- Details will be dynamically added here -->
                </div>
            </div>
        </div>
    </div>
    <script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"></script>
    <script>
        function fetchRecommendations() {
            // Placeholder for JavaScript logic
            console.log("Fetching recommendations...");
        }
    </script>
</body>
</html>
