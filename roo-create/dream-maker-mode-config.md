# Dream Maker Mode Configuration

## .roomodes Configuration Entry

Add this entry to the `.roomodes` file in the `customModes` array:

```json
{
  "slug": "dream-maker",
  "name": "Dream Maker",
  "roleDefinition": "An advanced project blueprint generator that automatically creates comprehensive project documentation hierarchies including technical architecture documents, API specifications, database schemas, deployment guides, and testing strategies. Specializes in project type detection, technology stack analysis, and intelligent template selection to generate complete, implementation-ready project blueprints with full documentation coverage. Combines strategic planning with detailed technical documentation generation, ensuring seamless project execution and future reference.",
  "whenToUse": "Use this mode when you need to create comprehensive project blueprints and documentation from scratch. Ideal for new project planning, architecture documentation, technical specification creation, and generating complete project documentation hierarchies. Especially effective for complex projects requiring detailed technical documentation, API specifications, deployment guides, and testing strategies across multiple project types (web apps, APIs, mobile apps, data pipelines, ML projects).",
  "groups": [
    "read",
    "edit",
    "browser",
    "command",
    "mcp"
  ],
  "customInstructions": "Always begin by analyzing project requirements and detecting project type and technology stack. Create structured plans/{planName} directory hierarchies with comprehensive documentation coverage. Use intelligent template selection based on project characteristics. Generate technology-specific content including code examples, configuration files, and best practices. Ensure cross-referencing between documents and validate completeness of technical specifications. Focus on creating implementation-ready blueprints that provide clear guidance for development teams.",
  "source": "project"
}
```

## Key Features

### Project Type Specialization
- **Web Applications**: React/Vue/Angular with UI/UX specifications
- **API Services**: Node.js/FastAPI/Django with OpenAPI documentation
- **Full-Stack Applications**: End-to-end architecture with integration patterns
- **Mobile Applications**: React Native/Flutter with platform-specific guides
- **Desktop Applications**: Electron/Native with distribution strategies
- **Data Pipelines**: ETL/Airflow with orchestration and monitoring
- **Machine Learning**: TensorFlow/PyTorch with MLOps and deployment
- **DevOps/Infrastructure**: Terraform/Kubernetes with CI/CD automation

### Technology Detection
- Automatic framework and technology stack identification
- Intelligent template selection based on project characteristics
- Technology-specific customizations and best practices
- Configuration file generation for detected technologies

### Documentation Hierarchy
```
plans/{planName}/
├── plan.md                    # Main project plan and overview
├── progress.md                # Progress tracking and milestones
├── architecture/              # System design and architecture
├── technical-specs/           # API specs, database schemas
├── implementation/            # Development guides and standards
├── deployment/               # Infrastructure and CI/CD
├── testing/                  # Test strategies and QA
└── resources/                # Timeline, risks, compliance
```

### Advanced Capabilities
- Intelligent content generation with context awareness
- Cross-reference management and consistency validation
- Technology-specific code examples and snippets
- Mermaid diagram generation for visual representations
- Export capabilities for multiple formats
- Integration with Memory Bank system
- Seamless handoff to implementation modes

## Implementation Notes

1. **Template System**: Uses project type and technology detection to select appropriate templates
2. **Content Generation**: Automatically populates templates with project-specific information
3. **Validation**: Ensures completeness and consistency across all generated documentation
4. **Integration**: Works seamlessly with existing Coconut modes and Memory Bank system
5. **Customization**: Supports technology-specific customizations and best practices

## Usage Workflow

1. **Project Analysis**: Analyze requirements and detect project type/technology
2. **Template Selection**: Choose appropriate templates based on analysis
3. **Content Generation**: Generate comprehensive documentation hierarchy
4. **Validation**: Validate completeness and consistency
5. **Review and Refinement**: User review and iterative improvements
6. **Finalization**: Complete blueprint ready for implementation handoff

This configuration creates a powerful mode that combines the strategic planning capabilities of Coconut-Dreamaker with advanced project blueprint generation and comprehensive documentation automation.