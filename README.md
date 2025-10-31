import React from 'react';
import { Container, Typography, Box, Paper, Grid, Chip } from '@mui/material';

function App() {
  return (
    <Container maxWidth="lg">
      <Box sx={{ my: 4 }}>
        <Typography variant="h2" component="h1" gutterBottom align="center">
          🏢 Enterprise MDM Platform
        </Typography>
        <Typography variant="h5" align="center" color="text.secondary" paragraph>
          Multi-Source Data Integration with ML-Based Entity Resolution
        </Typography>

        <Grid container spacing={3} sx={{ mt: 4 }}>
          <Grid item xs={12} md={3}>
            <Paper elevation={3} sx={{ p: 3, textAlign: 'center' }}>
              <Typography variant="h4" color="primary">5M+</Typography>
              <Typography variant="body1">Records Consolidated</Typography>
            </Paper>
          </Grid>
          <Grid item xs={12} md={3}>
            <Paper elevation={3} sx={{ p: 3, textAlign: 'center' }}>
              <Typography variant="h4" color="primary">15+</Typography>
              <Typography variant="body1">Source Systems</Typography>
            </Paper>
          </Grid>
          <Grid item xs={12} md={3}>
            <Paper elevation={3} sx={{ p: 3, textAlign: 'center' }}>
              <Typography variant="h4" color="primary">96%</Typography>
              <Typography variant="body1">Match Precision</Typography>
            </Paper>
          </Grid>
          <Grid item xs={12} md={3}>
            <Paper elevation={3} sx={{ p: 3, textAlign: 'center' }}>
              <Typography variant="h4" color="primary">94%</Typography>
              <Typography variant="body1">Data Quality</Typography>
            </Paper>
          </Grid>
        </Grid>

        <Box sx={{ mt: 6 }}>
          <Typography variant="h4" gutterBottom>Core Capabilities</Typography>
          
          <Paper elevation={2} sx={{ p: 3, mt: 2 }}>
            <Typography variant="h6">📊 Multi-Source Integration</Typography>
            <Typography variant="body2" sx={{ mt: 1, mb: 2 }}>
              Consolidate data from 15+ systems using Azure Data Factory, Databricks, and dbt
            </Typography>
            <Box sx={{ display: 'flex', gap: 1, flexWrap: 'wrap' }}>
              <Chip label="Salesforce" size="small" />
              <Chip label="SAP ERP" size="small" />
              <Chip label="REST APIs" size="small" />
              <Chip label="Kafka" size="small" />
              <Chip label="CSV Files" size="small" />
            </Box>
          </Paper>

          <Paper elevation={2} sx={{ p: 3, mt: 2 }}>
            <Typography variant="h6">🤖 ML-Based Entity Resolution</Typography>
            <Typography variant="body2" sx={{ mt: 1 }}>
              96% precision and 94% recall using fuzzy matching and probabilistic linking
            </Typography>
          </Paper>

          <Paper elevation={2} sx={{ p: 3, mt: 2 }}>
            <Typography variant="h6">✅ Data Quality Framework</Typography>
            <Typography variant="body2" sx={{ mt: 1, mb: 2 }}>
              Monitor 5 quality dimensions with Great Expectations (72% → 94% improvement)
            </Typography>
            <Box sx={{ display: 'flex', gap: 1, flexWrap: 'wrap' }}>
              <Chip label="Completeness: 98%" size="small" color="success" />
              <Chip label="Accuracy: 99.5%" size="small" color="success" />
              <Chip label="Consistency: 97%" size="small" color="success" />
              <Chip label="Timeliness: <1hr" size="small" color="success" />
              <Chip label="Uniqueness: 99.8%" size="small" color="success" />
            </Box>
          </Paper>

          <Paper elevation={2} sx={{ p: 3, mt: 2 }}>
            <Typography variant="h6">🔍 Data Governance</Typography>
            <Typography variant="body2" sx={{ mt: 1 }}>
              Azure Purview integration with data lineage, PII classification, and GDPR compliance
            </Typography>
          </Paper>
        </Box>

        <Box sx={{ mt: 6, textAlign: 'center' }}>
          <Typography variant="body2" color="text.secondary">
            Built by Neha Sharma | IIT Jodhpur
          </Typography>
          <Typography variant="body2" color="text.secondary">
            <a href="https://github.com/neha-iitjdh/mdm-platform">GitHub Repository</a>
          </Typography>
        </Box>
      </Box>
    </Container>
  );
}

export default App;
