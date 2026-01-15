<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Admin Panel - Content Management</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            background: #f5f5f5;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            overflow: hidden;
        }

        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .header h1 {
            font-size: 1.8rem;
        }

        .save-btn {
            background: white;
            color: #667eea;
            border: none;
            padding: 0.8rem 2rem;
            border-radius: 5px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.2s;
        }

        .save-btn:hover {
            transform: scale(1.05);
        }

        .tabs {
            display: flex;
            background: #f8f9fa;
            border-bottom: 2px solid #e9ecef;
        }

        .tab {
            padding: 1rem 2rem;
            cursor: pointer;
            border: none;
            background: none;
            font-size: 1rem;
            transition: all 0.3s;
        }

        .tab:hover {
            background: #e9ecef;
        }

        .tab.active {
            background: white;
            border-bottom: 3px solid #667eea;
            font-weight: bold;
        }

        .content {
            padding: 2rem;
        }

        .tab-content {
            display: none;
        }

        .tab-content.active {
            display: block;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: #333;
        }

        input[type="text"],
        input[type="email"],
        input[type="url"],
        textarea {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
            font-family: inherit;
        }

        textarea {
            min-height: 100px;
            resize: vertical;
        }

        .section-title {
            font-size: 1.5rem;
            color: #667eea;
            margin-bottom: 1.5rem;
            padding-bottom: 0.5rem;
            border-bottom: 2px solid #e9ecef;
        }

        .item-list {
            border: 1px solid #ddd;
            border-radius: 5px;
            margin-bottom: 1.5rem;
        }

        .item {
            padding: 1rem;
            border-bottom: 1px solid #ddd;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .item:last-child {
            border-bottom: none;
        }

        .item-content {
            flex: 1;
        }

        .item-title {
            font-weight: bold;
            margin-bottom: 0.25rem;
        }

        .item-subtitle {
            color: #666;
            font-size: 0.9rem;
        }

        .item-actions {
            display: flex;
            gap: 0.5rem;
        }

        .btn {
            padding: 0.5rem 1rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 0.9rem;
            transition: opacity 0.2s;
        }

        .btn:hover {
            opacity: 0.8;
        }

        .btn-edit {
            background: #667eea;
            color: white;
        }

        .btn-delete {
            background: #dc3545;
            color: white;
        }

        .btn-add {
            background: #28a745;
            color: white;
            padding: 0.8rem 1.5rem;
            font-size: 1rem;
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.5);
            z-index: 1000;
            align-items: center;
            justify-content: center;
        }

        .modal.active {
            display: flex;
        }

        .modal-content {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            max-width: 600px;
            width: 90%;
            max-height: 90vh;
            overflow-y: auto;
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1.5rem;
        }

        .modal-header h2 {
            color: #667eea;
        }

        .close-btn {
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: #999;
        }

        .close-btn:hover {
            color: #333;
        }

        .alert {
            padding: 1rem;
            border-radius: 5px;
            margin-bottom: 1rem;
            display: none;
        }

        .alert.active {
            display: block;
        }

        .alert-success {
            background: #d4edda;
            color: #155724;
            border: 1px solid #c3e6cb;
        }

        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1rem;
        }

        @media (max-width: 768px) {
            .grid-2 {
                grid-template-columns: 1fr;
            }
            
            .tabs {
                overflow-x: auto;
            }
            
            .tab {
                padding: 1rem;
                white-space: nowrap;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>📝 Website Admin Panel</h1>
            <button class="save-btn" onclick="saveAllData()">💾 Save All Changes</button>
        </div>

        <div class="alert alert-success" id="saveAlert">
            ✅ Changes saved successfully!
        </div>

        <div class="tabs">
            <button class="tab active" onclick="switchTab('profile')">Profile</button>
            <button class="tab" onclick="switchTab('experience')">Experience</button>
            <button class="tab" onclick="switchTab('education')">Education</button>
            <button class="tab" onclick="switchTab('skills')">Skills</button>
            <button class="tab" onclick="switchTab('books')">Books</button>
            <button class="tab" onclick="switchTab('blog')">Blog</button>
            <button class="tab" onclick="switchTab('contact')">Contact</button>
        </div>

        <div class="content">
            <!-- Profile Tab -->
            <div id="profile" class="tab-content active">
                <h2 class="section-title">Profile Information</h2>
                <div class="form-group">
                    <label>Your Name</label>
                    <input type="text" id="profileName" placeholder="Enter your full name">
                </div>
                <div class="form-group">
                    <label>Profession</label>
                    <input type="text" id="profileProfession" placeholder="e.g., Software Developer">
                </div>
                <div class="form-group">
                    <label>About You</label>
                    <textarea id="profileAbout" placeholder="Tell visitors about yourself and your interests..."></textarea>
                </div>
            </div>

            <!-- Experience Tab -->
            <div id="experience" class="tab-content">
                <h2 class="section-title">Work Experience</h2>
                <button class="btn btn-add" onclick="openModal('experience')">+ Add Experience</button>
                <div class="item-list" id="experienceList"></div>
            </div>

            <!-- Education Tab -->
            <div id="education" class="tab-content">
                <h2 class="section-title">Education</h2>
                <button class="btn btn-add" onclick="openModal('education')">+ Add Education</button>
                <div class="item-list" id="educationList"></div>
            </div>

            <!-- Skills Tab -->
            <div id="skills" class="tab-content">
                <h2 class="section-title">Skills</h2>
                <div class="form-group">
                    <label>Enter your skills (comma-separated)</label>
                    <textarea id="skillsInput" placeholder="JavaScript, Python, React, Design, etc."></textarea>
                    <small style="color: #666;">Separate each skill with a comma</small>
                </div>
            </div>

            <!-- Books Tab -->
            <div id="books" class="tab-content">
                <h2 class="section-title">Favorite Books</h2>
                <button class="btn btn-add" onclick="openModal('book')">+ Add Book</button>
                <div class="item-list" id="booksList"></div>
            </div>

            <!-- Blog Tab -->
            <div id="blog" class="tab-content">
                <h2 class="section-title">Blog Posts</h2>
                <button class="btn btn-add" onclick="openModal('blog')">+ Add Blog Post</button>
                <div class="item-list" id="blogList"></div>
            </div>

            <!-- Contact Tab -->
            <div id="contact" class="tab-content">
                <h2 class="section-title">Contact Information</h2>
                <div class="grid-2">
                    <div class="form-group">
                        <label>Email</label>
                        <input type="email" id="contactEmail" placeholder="your.email@example.com">
                    </div>
                    <div class="form-group">
                        <label>LinkedIn</label>
                        <input type="url" id="contactLinkedin" placeholder="linkedin.com/in/yourprofile">
                    </div>
                    <div class="form-group">
                        <label>GitHub</label>
                        <input type="url" id="contactGithub" placeholder="github.com/yourusername">
                    </div>
                    <div class="form-group">
                        <label>Twitter/X</label>
                        <input type="text" id="contactTwitter" placeholder="@yourhandle">
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal for Adding/Editing Items -->
    <div class="modal" id="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h2 id="modalTitle">Add Item</h2>
                <button class="close-btn" onclick="closeModal()">&times;</button>
            </div>
            <div id="modalBody"></div>
            <button class="btn btn-add" onclick="saveModalData()" style="width: 100%; margin-top: 1rem;">Save</button>
        </div>
    </div>

    <script>
        let currentModalType = '';
        let editingIndex = -1;
        let data = {
            profile: { name: '', profession: '', about: '' },
            experience: [],
            education: [],
            skills: [],
            books: [],
            blog: [],
            contact: { email: '', linkedin: '', github: '', twitter: '' }
        };

        function loadData() {
            const saved = localStorage.getItem('websiteData');
            if (saved) {
                data = JSON.parse(saved);
                populateFields();
            }
        }

        function populateFields() {
            document.getElementById('profileName').value = data.profile.name || '';
            document.getElementById('profileProfession').value = data.profile.profession || '';
            document.getElementById('profileAbout').value = data.profile.about || '';
            document.getElementById('skillsInput').value = data.skills.join(', ');
            document.getElementById('contactEmail').value = data.contact.email || '';
            document.getElementById('contactLinkedin').value = data.contact.linkedin || '';
            document.getElementById('contactGithub').value = data.contact.github || '';
            document.getElementById('contactTwitter').value = data.contact.twitter || '';
            
            renderList('experience');
            renderList('education');
            renderList('books');
            renderList('blog');
        }

        function switchTab(tabName) {
            document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
            document.querySelectorAll('.tab-content').forEach(c => c.classList.remove('active'));
            event.target.classList.add('active');
            document.getElementById(tabName).classList.add('active');
        }

        function openModal(type) {
            currentModalType = type;
            editingIndex = -1;
            const modal = document.getElementById('modal');
            const modalBody = document.getElementById('modalBody');
            const modalTitle = document.getElementById('modalTitle');
            
            let html = '';
            
            if (type === 'experience') {
                modalTitle.textContent = 'Add Work Experience';
                html = `
                    <div class="form-group">
                        <label>Job Title</label>
                        <input type="text" id="modalInput1" placeholder="e.g., Senior Developer">
                    </div>
                    <div class="form-group">
                        <label>Company Name</label>
                        <input type="text" id="modalInput2" placeholder="e.g., Tech Corp">
                    </div>
                    <div class="form-group">
                        <label>Duration</label>
                        <input type="text" id="modalInput3" placeholder="e.g., 2020 - Present">
                    </div>
                    <div class="form-group">
                        <label>Description</label>
                        <textarea id="modalInput4" placeholder="Describe your role and achievements..."></textarea>
                    </div>
                `;
            } else if (type === 'education') {
                modalTitle.textContent = 'Add Education';
                html = `
                    <div class="form-group">
                        <label>Degree</label>
                        <input type="text" id="modalInput1" placeholder="e.g., Bachelor of Science">
                    </div>
                    <div class="form-group">
                        <label>Institution</label>
                        <input type="text" id="modalInput2" placeholder="e.g., University Name">
                    </div>
                    <div class="form-group">
                        <label>Duration</label>
                        <input type="text" id="modalInput3" placeholder="e.g., 2014 - 2018">
                    </div>
                    <div class="form-group">
                        <label>Description</label>
                        <textarea id="modalInput4" placeholder="Major, achievements, relevant coursework..."></textarea>
                    </div>
                `;
            } else if (type === 'book') {
                modalTitle.textContent = 'Add Favorite Book';
                html = `
                    <div class="form-group">
                        <label>Book Title</label>
                        <input type="text" id="modalInput1" placeholder="Enter book title">
                    </div>
                    <div class="form-group">
                        <label>Author</label>
                        <input type="text" id="modalInput2" placeholder="Author name">
                    </div>
                    <div class="form-group">
                        <label>Your Review/Thoughts</label>
                        <textarea id="modalInput3" placeholder="Why do you love this book?"></textarea>
                    </div>
                `;
            } else if (type === 'blog') {
                modalTitle.textContent = 'Add Blog Post';
                html = `
                    <div class="form-group">
                        <label>Post Title</label>
                        <input type="text" id="modalInput1" placeholder="Enter post title">
                    </div>
                    <div class="form-group">
                        <label>Date</label>
                        <input type="text" id="modalInput2" placeholder="e.g., January 15, 2026">
                    </div>
                    <div class="form-group">
                        <label>Content Preview</label>
                        <textarea id="modalInput3" placeholder="Write a preview or full content of your blog post..."></textarea>
                    </div>
                `;
            }
            
            modalBody.innerHTML = html;
            modal.classList.add('active');
        }

        function closeModal() {
            document.getElementById('modal').classList.remove('active');
        }

        function saveModalData() {
            const input1 = document.getElementById('modalInput1').value;
            const input2 = document.getElementById('modalInput2').value;
            const input3 = document.getElementById('modalInput3').value;
            const input4 = document.getElementById('modalInput4')?.value;
            
            if (!input1 || !input2) {
                alert('Please fill in all required fields');
                return;
            }
            
            let item = {};
            
            if (currentModalType === 'experience') {
                item = { title: input1, company: input2, duration: input3, description: input4 };
            } else if (currentModalType === 'education') {
                item = { degree: input1, institution: input2, duration: input3, description: input4 };
            } else if (currentModalType === 'book') {
                item = { title: input1, author: input2, review: input3 };
            } else if (currentModalType === 'blog') {
                item = { title: input1, date: input2, content: input3 };
            }
            
            if (editingIndex >= 0) {
                data[currentModalType][editingIndex] = item;
            } else {
                data[currentModalType].push(item);
            }
            
            renderList(currentModalType);
            closeModal();
            saveAllData();
        }

        function renderList(type) {
            const listId = type === 'experience' ? 'experienceList' : 
                          type === 'education' ? 'educationList' : 
                          type === 'books' ? 'booksList' : 'blogList';
            const list = document.getElementById(listId);
            
            if (!data[type] || data[type].length === 0) {
                list.innerHTML = '<div class="item"><p style="color: #999;">No items added yet</p></div>';
                return;
            }
            
            list.innerHTML = data[type].map((item, index) => {
                let title, subtitle;
                
                if (type === 'experience') {
                    title = item.title;
                    subtitle = `${item.company} | ${item.duration}`;
                } else if (type === 'education') {
                    title = item.degree;
                    subtitle = `${item.institution} | ${item.duration}`;
                } else if (type === 'books') {
                    title = item.title;
                    subtitle = `by ${item.author}`;
                } else if (type === 'blog') {
                    title = item.title;
                    subtitle = item.date;
                }
                
                return `
                    <div class="item">
                        <div class="item-content">
                            <div class="item-title">${title}</div>
                            <div class="item-subtitle">${subtitle}</div>
                        </div>
                        <div class="item-actions">
                            <button class="btn btn-edit" onclick="editItem('${type}', ${index})">Edit</button>
                            <button class="btn btn-delete" onclick="deleteItem('${type}', ${index})">Delete</button>
                        </div>
                    </div>
                `;
            }).join('');
        }

        function editItem(type, index) {
            editingIndex = index;
            currentModalType = type;
            const item = data[type][index];
            
            openModal(type);
            
            setTimeout(() => {
                if (type === 'experience') {
                    document.getElementById('modalInput1').value = item.title;
                    document.getElementById('modalInput2').value = item.company;
                    document.getElementById('modalInput3').value = item.duration;
                    document.getElementById('modalInput4').value = item.description;
                } else if (type === 'education') {
                    document.getElementById('modalInput1').value = item.degree;
                    document.getElementById('modalInput2').value = item.institution;
                    document.getElementById('modalInput3').value = item.duration;
                    document.getElementById('modalInput4').value = item.description;
                } else if (type === 'books') {
                    document.getElementById('modalInput1').value = item.title;
                    document.getElementById('modalInput2').value = item.author;
                    document.getElementById('modalInput3').value = item.review;
                } else if (type === 'blog') {
                    document.getElementById('modalInput1').value = item.title;
                    document.getElementById('modalInput2').value = item.date;
                    document.getElementById('modalInput3').value = item.content;
                }
                document.getElementById('modalTitle').textContent = 'Edit ' + type.charAt(0).toUpperCase() + type.slice(1);
            }, 100);
        }

        function deleteItem(type, index) {
            if (confirm('Are you sure you want to delete this item?')) {
                data[type].splice(index, 1);
                renderList(type);
                saveAllData();
            }
        }

        function saveAllData() {
            data.profile.name = document.getElementById('profileName').value;
            data.profile.profession = document.getElementById('profileProfession').value;
            data.profile.about = document.getElementById('profileAbout').value;
            data.skills = document.getElementById('skillsInput').value.split(',').map(s => s.trim()).filter(s => s);
            data.contact.email = document.getElementById('contactEmail').value;
            data.contact.linkedin = document.getElementById('contactLinkedin').value;
            data.contact.github = document.getElementById('contactGithub').value;
            data.contact.twitter = document.getElementById('contactTwitter').value;
            
            localStorage.setItem('websiteData', JSON.stringify(data));
            
            const alert = document.getElementById('saveAlert');
            alert.classList.add('active');
            setTimeout(() => alert.classList.remove('active'), 3000);
        }

        window.onload = loadData;
    </script>
</body>
</html>
